# Security Policy

## Supported Versions

This project is currently in active development. Security fixes are applied to the latest version only.

| Version | Supported          |
| ------- | ------------------ |
| latest  | ✅ Yes             |
| older   | ❌ No              |

## Reporting a Vulnerability

**Please do NOT report security vulnerabilities through public GitHub issues.**

If you discover a security vulnerability in GymFlow AI, please report it responsibly:

1. **Email**: Send a detailed report to the repository owner via GitHub's private contact mechanism.
2. **Subject Line**: Use `[SECURITY] GymFlow AI - <brief description>`.
3. **Include**:
   - Description of the vulnerability and its potential impact.
   - Steps to reproduce the issue.
   - Any suggested fix or mitigation (optional but appreciated).

## What to Expect

- **Acknowledgement**: You will receive an acknowledgement within 48 hours.
- **Assessment**: We will assess the severity and impact within 7 days.
- **Resolution**: We aim to release a fix within 30 days of a confirmed vulnerability.
- **Credit**: With your permission, we will credit you in the release notes.

## Security Best Practices for Users

When deploying GymFlow AI:

- **Never** commit `.env` files or any file containing real API keys to Git.
- **Always** use the `.env.example` as a template and store real credentials separately.
- **Rotate** all API keys and tokens immediately if you suspect they have been exposed.
- **Restrict** database access using Row Level Security (RLS) in Supabase.
- **Secure** your n8n instance with authentication and HTTPS.
- **Review** n8n workflow credentials after import and update all placeholder values.

## Credential Handling in This Repository

All workflow JSON files in this repository have been sanitized:
- Real API tokens have been replaced with `YOUR_CHATWOOT_API_ACCESS_TOKEN` placeholder.
- No real passwords, tokens, or private keys are stored in this repository.
- Credential IDs in n8n JSON (e.g., `"id": "N7FZ70HUMYaZ3QxO"`) are n8n-internal references and do not expose actual secrets.
