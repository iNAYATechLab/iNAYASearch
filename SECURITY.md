# Security Policy

## Security at iNAYASearch

Security is a core requirement of iNAYASearch.

The project handles untrusted web content, URLs, network requests, search queries, documents, and potentially large amounts of external data. Security must therefore be considered throughout the crawler, parser, indexer, query engine, API, web interface, infrastructure, and operational systems.

## Supported Versions

During active development, security fixes are generally applied to the current development version.

Once stable releases are established, supported versions and their security-maintenance periods will be documented here.

## Reporting a Vulnerability

Please do not publicly disclose an unpatched security vulnerability through a GitHub issue, pull request, discussion, or other public project channel.

Report security vulnerabilities privately to the project maintainers through an appropriate private GitHub security reporting mechanism when available.

If private security reporting is not available, contact the project maintainers through the repository's available private communication channel.

## What to Include

A useful security report should include, when possible:

- A clear description of the vulnerability.
- The affected component.
- The affected version or commit.
- The security impact.
- Steps required to reproduce the issue.
- A minimal proof of concept when safe to provide.
- Any relevant logs or error messages.
- A suggested mitigation or fix, if known.

Do not include real passwords, access tokens, private keys, personal data, or other sensitive credentials in a security report.

## Security Vulnerability Examples

Security reports may include issues such as:

- Server-Side Request Forgery (SSRF).
- Remote Code Execution.
- Authentication bypass.
- Authorization bypass.
- Cross-Site Scripting (XSS).
- Injection vulnerabilities.
- Unsafe HTML or document processing.
- Malicious redirects.
- URL validation bypasses.
- Crawler abuse.
- Resource exhaustion.
- Denial-of-Service conditions.
- Sensitive information disclosure.
- Credential or secret exposure.
- Insecure file processing.
- Index corruption caused by malicious input.
- Query abuse.
- Security weaknesses in administrative interfaces.
- Dependency or supply-chain vulnerabilities.

This list is not exhaustive.

## Crawler Security

The crawler is an especially security-sensitive component.

Crawler-related implementations must consider:

- SSRF protection.
- URL validation.
- Redirect validation.
- Network access restrictions.
- Private and internal network addresses.
- DNS-related risks.
- Resource limits.
- Request timeouts.
- Response size limits.
- Content-type validation.
- Malicious or malformed documents.
- Abuse prevention.
- Per-domain request controls.

Crawler functionality must never assume that remote URLs or remote content are trustworthy.

## Secrets and Credentials

Never commit the following to the repository:

- Passwords.
- API keys.
- Access tokens.
- Private keys.
- Database credentials.
- Session secrets.
- Encryption keys.
- Cloud credentials.
- Personal authentication credentials.
- Production secrets.

Use appropriate environment variables or secure secret-management mechanisms for sensitive configuration.

## Security by Design

Security should be considered before implementation rather than added only after a vulnerability is discovered.

Security-sensitive changes should consider:

1. Input validation.
2. Authentication and authorization.
3. Trust boundaries.
4. Resource limits.
5. Error handling.
6. Logging and monitoring.
7. Abuse prevention.
8. Data protection.
9. Dependency risks.
10. Failure behavior.

## Responsible Disclosure

Security researchers and contributors are encouraged to report vulnerabilities responsibly.

Please allow maintainers reasonable time to investigate and address a vulnerability before publicly disclosing technical details.

## Security Updates

Resolved security issues may be documented through:

- Security advisories.
- Changelog entries.
- Release notes.
- Security-related documentation.

Sensitive exploitation details should not be published unnecessarily.

## Security Contact

The project will use the repository's configured private security reporting and maintainer communication mechanisms for vulnerability handling.

Security reports should not be submitted through public issue trackers when they contain sensitive vulnerability details.