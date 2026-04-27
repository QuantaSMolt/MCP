# Security Policy

## Reporting Security Issues

If you discover a security vulnerability, please report it privately.

## Credentials

- All credentials must be stored in 1Password, never in code
- No credential values in git history
- Use environment variables or secure vault references

## SSH Access

- Key-based authentication only
- No password authentication
- Root login disabled in production
- Regular key rotation required

## GitHub

- Branch protection enabled on main
- 1 reviewer required for merges
- No force push allowed
- Secret scanning enabled

## Development Practices

1. Never commit secrets
2. Use .gitignore for sensitive files
3. Review code before committing
4. Test in staging before production

## Agent Credentials

Agents access credentials via:
- 1Password CLI (service account)
- GitHub MCP (scoped tokens)
- No direct credential storage in agent configs

## Incident Response

If credentials are compromised:
1. Revoke immediately in platform
2. Update 1Password
3. Rotate affected services
4. Document incident

---
Last updated: 2026-04-26
