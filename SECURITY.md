# Security Policy

## Supported Versions

The following versions of Demoappaz204 are currently being supported with security updates:

| Version | Supported          | .NET Version | Status |
| ------- | ------------------ | ------------ | ------ |
| 1.2.x   | :white_check_mark: | .NET 8.0     | Current |
| 1.1.x   | :white_check_mark: | .NET 8.0     | LTS     |
| 1.0.x   | :warning:          | .NET 8.0     | Limited Support |
| < 1.0   | :x:                | .NET 7.0     | End of Life |

**Note**: We recommend always using the latest stable version for the best security posture.

## Security Best Practices

Before reporting a vulnerability, please ensure you've followed these security best practices:

- Keep your Azure services and dependencies up to date
- Use HTTPS for all communications
- Implement proper input validation
- Follow the principle of least privilege for Azure resources
- Enable Azure Security Center recommendations
- Use managed identities where possible

## Reporting a Vulnerability

### Internal Reporting Process (TechM Team Members)

**Step 1: Internal Discussion**
1. **Teams Channel**: Post your security concern in the dedicated **#demoappaz204-security** Teams channel
   - Use the format: `🔒 SECURITY: [Brief Description]`
   - Include severity level: `Critical`, `High`, `Medium`, or `Low`
   - Tag relevant team members: `@security-team` `@project-leads`

2. **Initial Assessment**: The security team will acknowledge within **2 business hours** and provide initial assessment within **24 hours**

3. **Internal Discussion**: 
   - Security team will create a private discussion thread
   - Include technical details, impact assessment, and reproduction steps
   - Collaborate on potential fixes and mitigation strategies

**Step 2: Create Pull Request**
1. **Branch Creation**: Create a security fix branch using the naming convention:
   ```
   security/[issue-id]-[brief-description]
   Example: security/SEC-001-sql-injection-fix
   ```

2. **Pull Request Guidelines**:
   - **Title**: `🔒 [SECURITY] Brief description of the fix`
   - **Description**: Reference the Teams discussion and include:
     - Vulnerability description and impact
     - Fix implementation details
     - Testing performed
     - Security team approval reference
   - **Reviewers**: Assign to security team and project leads
   - **Labels**: Add `security`, `priority-high`, and appropriate severity label

3. **Review Process**:
   - Security team review: **Required**
   - Code review by 2+ senior developers: **Required**
   - Automated security scans: **Must pass**
   - Manual testing: **Required for critical/high severity**

### External Reporting Process

**For External Contributors or Security Researchers:**

1. **Email**: Send detailed vulnerability reports to: `security@techm-demoapp.com`
2. **Information to Include**:
   - Detailed description of the vulnerability
   - Steps to reproduce the issue
   - Potential impact assessment
   - Suggested remediation (if any)
   - Your contact information for follow-up

3. **Response Timeline**:
   - **Initial acknowledgment**: Within 48 hours
   - **Preliminary assessment**: Within 5 business days
   - **Status updates**: Weekly or as significant developments occur
   - **Resolution timeline**: Based on severity (see table below)

## Vulnerability Response Timeline

| Severity | Initial Response | Fix Target | Deployment Target |
|----------|------------------|------------|-------------------|
| Critical | 2 hours          | 24 hours   | 48 hours         |
| High     | 8 hours          | 72 hours   | 1 week           |
| Medium   | 24 hours         | 2 weeks    | 1 month          |
| Low      | 48 hours         | 1 month    | Next release     |

## Security Contact Information

- **Primary Security Contact**: security-lead@techm.com
- **Teams Channel**: #demoappaz204-security
- **Emergency Contact**: +1-XXX-XXX-XXXX (for critical vulnerabilities only)
- **PGP Key**: Available upon request for encrypted communications

## Disclosure Policy

- **Coordinated Disclosure**: We practice coordinated disclosure and ask that you do not publicly disclose vulnerabilities until we've had a chance to address them
- **Recognition**: Security researchers will be credited in our security acknowledgments (unless they prefer to remain anonymous)
- **Bug Bounty**: Currently evaluating a bug bounty program - stay tuned for updates

## Security Resources

- [Azure Security Documentation](https://docs.microsoft.com/en-us/azure/security/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [ASP.NET Core Security Guidelines](https://docs.microsoft.com/en-us/aspnet/core/security/)
- [Bicep Security Best Practices](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/best-practices)

---

**Last Updated**: February 3, 2026  
**Next Review**: May 3, 2026


