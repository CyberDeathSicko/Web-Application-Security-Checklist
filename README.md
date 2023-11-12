# Web Application Security Testing Checklist

Welcome to the Web Application Security Testing Checklist repository. This checklist serves as a comprehensive guide for ensuring the security of your web applications. Whether you're a seasoned professional or just starting, use this checklist to navigate through various security testing aspects.

## Recon on Wildcard Domain

### Subdomain Enumeration
- Leverage tools like amass, subfinder, assetfinder, dnsgen, and massdns.
- Utilize diverse wordlists and permutations for subdomain discovery.
- Scrutinize DNS records for wildcard entries and potential subdomains.

### SSL/TLS Certificate Analysis
- Use CT logs (crt.sh) for certificate transparency.
- Examine wildcard certificates, including expiration dates and issuer details.

### Search Engine Dorking
- Conduct targeted Google searches with advanced operators for subdomain discovery.
- Utilize tools like Shodan and ZoomEye for exposed services.

### Web Archives
- Utilize the Wayback Machine to view historical files like robots.txt and URLs.

## Network Information

### BGP Lookup
- Use BGP Lookup tools like bgp.he.net for checking IP target information.
- Perform DNS-related checks using tools like DNSDumpster and DigWebInterface.

### Subdomain Takeover
- Utilize tools like Can I Take Over XYZ to check for subdomain takeover opportunities.

### Passive Reconnaissance
- Use Google Dorks for reconnaissance with advanced search operators.
- Leverage threat intelligence gathering tools like theHarvester.
- Perform WHOIS Lookup to gather domain registration information.
- Analyze robots.txt for insights into the site's structure.
- Spider the website for URLs using tools like gobuster.
- Conduct DNS Enumeration using tools like dnsrecon.

### Active Reconnaissance
- Conduct advanced port scanning using Nmap.
- Perform service fingerprinting with banner grabbing.
- Utilize network sniffing fingerprinting using Nmap scripts.
- Check for subdomain takeover using tools like subjack.
- Scan the web application using tools like nikto and gobuster.
- Conduct SSL/TLS vulnerability checks with testssl.sh.
- Verify HTTP security headers using gobuster.

## Bug Testing

### Injection Vulnerabilities
- Test for SQL injection vulnerabilities.
- Check for OS command injection vulnerabilities.
- Assess LDAP injection vulnerabilities.

### Cross-Site Scripting (XSS)
- Test for reflected XSS vulnerabilities.
- Check for stored XSS vulnerabilities.
- Assess DOM-based XSS vulnerabilities.

### Cross-Site Request Forgery (CSRF)
- Test for CSRF vulnerabilities.
- Verify the effectiveness of CSRF protection mechanisms.

### Security Misconfigurations
- Check for exposed sensitive information.
- Test for default credentials on administrative interfaces.
- Verify secure configuration of cloud services.

### Insecure Direct Object References (IDOR)
- Test for IDOR vulnerabilities.
- Verify that users cannot access unauthorized resources.

### Server-Side Request Forgery (SSRF)
- Test for SSRF vulnerabilities.
- Verify that the application filters or blocks malicious requests.

### File Upload Security
- Test for unrestricted file uploads.
- Check for proper validation of file types and content.
- Verify secure storage and access controls for uploaded files.

### XML External Entity (XXE) Injection
- Test for XXE vulnerabilities in XML parsing.
- Verify that XML inputs are properly validated and sanitized.

### Security Headers
- Check for the presence and effectiveness of security headers.
- Include headers such as Content Security Policy (CSP) and Strict-Transport-Security (HSTS).

### Clickjacking
- Test for clickjacking vulnerabilities.
- Verify that UI elements cannot be embedded in iframes without proper controls.

### Business Logic Testing
- Test for logical flaws in the application workflow.
- Verify the enforcement of business rules and access controls.
- Assess the impact of parameter manipulation on business processes.

### Cryptographic Vulnerabilities
- Check for weak or deprecated cryptographic algorithms.
- Verify the secure storage and transmission of sensitive information.

### Mobile-specific Vulnerabilities
- Test for mobile application-specific vulnerabilities.
- Verify the security of APIs used by mobile applications.
- Assess the storage and handling of sensitive information on mobile devices.

### API Security
- Test the security of APIs for vulnerabilities.
- Verify proper authentication and authorization mechanisms.
- Assess the handling of input data and error messages.

### IoT-specific Vulnerabilities
- Test for security vulnerabilities in IoT devices.
- Assess the communication security of IoT devices.
- Verify the security of firmware and update mechanisms.

**Feel free to contribute and improve this checklist for the benefit of the community.**

## Contributors
- [Your Name]
- [Other Security Researchers]
