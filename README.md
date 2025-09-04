# Test Repository with Vulnerabilities
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCampus-Media%2Ftest-repo-with-vulns.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FCampus-Media%2Ftest-repo-with-vulns?ref=badge_shield)


⚠️ **WARNING: This repository contains intentionally vulnerable dependencies for testing purposes only!**

This repository is designed to test security scanning tools like SBOM-Link. It contains:

## Vulnerable Dependencies

- **lodash 4.17.15** - Prototype pollution vulnerability (CVE-2021-23337)
- **axios 0.21.1** - Server-Side Request Forgery (CVE-2021-3749)
- **moment 2.29.1** - Regular Expression Denial of Service (ReDoS)
- **express 4.17.1** - Various CVEs including path traversal
- **jquery 3.6.0** - Cross-Site Scripting (XSS) vulnerabilities
- **bootstrap 4.6.0** - XSS vulnerabilities
- **react 16.14.0** - Various security vulnerabilities

## Vulnerable Code Examples

The application includes intentionally vulnerable code patterns:

1. **Prototype Pollution** - Using lodash.merge with user input
2. **SSRF** - Making HTTP requests with user-controlled URLs
3. **ReDoS** - Using moment.js with user-controlled date strings
4. **Path Traversal** - File upload without proper validation
5. **XSS** - Using vulnerable frontend libraries

## Usage

```bash
npm install
npm start
```

The app will run on port 3000 and expose vulnerable endpoints.

## Testing SBOM-Link Integration

1. Install the SBOM-Link GitHub App on this repository
2. Push code changes to trigger security scans
3. Check for policy violations in the SBOM-Link dashboard
4. Verify that vulnerable dependencies are detected

## Security Notes

- This repository should NEVER be used in production
- All vulnerabilities are intentional for testing purposes
- Do not deploy this code to any public-facing environment
- Use only in isolated testing environments

## Expected SBOM-Link Findings

When scanned by SBOM-Link, this repository should generate:

- High/Critical severity alerts for vulnerable dependencies
- Policy violations for outdated packages
- Security recommendations for dependency updates
- Risk score calculations based on vulnerability data # Test webhook
# Webhook test Sun Jun 22 16:30:41 PDT 2025
# Testing webhook fix - Sun Jun 22 17:01:39 PDT 2025
# Final webhook test - Sun Jun 22 17:07:24 PDT 2025
# Testing updated webhook URL - Sun Jun 22 17:10:00 PDT 2025
# Final webhook test - Sun Jun 22 18:10:47 PDT 2025
# Webhook URL test - Mon Jun 23 09:08:10 PDT 2025
# Testing push event handling - Mon Jun 23 09:56:42 PDT 2025


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCampus-Media%2Ftest-repo-with-vulns.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FCampus-Media%2Ftest-repo-with-vulns?ref=badge_large)