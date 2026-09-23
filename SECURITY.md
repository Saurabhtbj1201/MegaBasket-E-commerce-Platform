# Security Policy

The MegaBasket team takes security and privacy very seriously. We appreciate your efforts to responsibly disclose any vulnerabilities you find.

---

## Supported Versions

We provide security updates and patches for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | :white_check_mark: |
| < 1.0   | :x:                |

---

## Reporting a Vulnerability

If you discover a security vulnerability within **MegaBasket E-Commerce Platform**, please do **NOT** report it publicly through a GitHub issue or public forum.

Instead, please send an email directly to:

📧 **[megabasket.v01@gmail.com](mailto:megabasket.v01@gmail.com)**

### What to include in your report:

To help us triage and resolve the issue quickly, please provide:
1. **Description**: Clear description of the vulnerability and its potential impact.
2. **Steps to Reproduce**: Detailed reproduction steps, including sample requests, endpoints, or payload.
3. **Proof of Concept (PoC)**: Minimal code or screen recording demonstrating the vulnerability.
4. **Environment**: Affected branch, commit hash, operating system, and browser or API client.
5. **Mitigation Suggestion**: Any proposed fix or mitigation, if available.

---

## Response & Disclosure Process

1. **Acknowledgment**: You will receive an initial response acknowledging receipt within **48 hours**.
2. **Investigation & Triage**: Our team will assess the report and verify the vulnerability.
3. **Patch Development**: A fix will be developed, tested, and prepared for release.
4. **Coordinated Disclosure**: Once the fix is deployed, we will acknowledge your contribution (if desired) and publish relevant release notes.

---

## Security Best Practices for MegaBasket Deployment

When deploying MegaBasket to production (e.g., [Vercel](https://vercel.com/) for frontend, [Azure App Service](https://azure.microsoft.com/) for backend, [MongoDB Atlas](https://www.mongodb.com/atlas)):

- **Environment Variables**: Never check `.env` files into source control. Store secrets in Azure Application Settings, Vercel Environment Variables, or GitHub Secrets.
- **JWT Secret**: Use a cryptographically strong, random secret key for `JWT_SECRET`.
- **Database Access**: Restrict MongoDB Atlas IP access lists to trusted hosts only.
- **AWS S3 Permissions**: Restrict S3 bucket policies to allow public read only for uploaded assets, and keep AWS credentials strictly restricted with least-privilege IAM policies.
- **HTTPS**: Always enforce HTTPS in production environments.
- **CORS**: Configure `CORS_ORIGIN` to only allow trusted domains (e.g. `https://megabasket.vercel.app`).
