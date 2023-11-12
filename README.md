# Web Application Security Testing Checklist

Welcome to the Web Application Security Testing Checklist repository. This checklist serves as a comprehensive guide for ensuring the security of your web applications. Whether you're a seasoned professional or just starting, use this checklist to navigate through various security testing aspects.

<details>
<summary style="color: #3498db; font-size: 18px;"><strong>Recon on Wildcard Domain</strong></summary>
<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Subdomain Enumeration</strong></summary>

- Leverage tools like amass, subfinder, assetfinder, dnsgen, and massdns.
- Utilize diverse wordlists and permutations for subdomain discovery.
- Scrutinize DNS records for wildcard entries and potential subdomains.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>SSL/TLS Certificate Analysis</strong></summary>

- Use CT logs (crt.sh) for certificate transparency.
- Examine wildcard certificates, including expiration dates and issuer details.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Search Engine Dorking</strong></summary>

- Conduct targeted Google searches with advanced operators for subdomain discovery.
- Utilize tools like Shodan and ZoomEye for exposed services.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Web Archives</strong></summary>

- Utilize the Wayback Machine to view historical files like robots.txt and URLs.
</details>
</details>

<details>
<summary style="color: #3498db; font-size: 18px;"><strong>Network Information</strong></summary>
<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>BGP Lookup</strong></summary>

- Use BGP Lookup tools like bgp.he.net for checking IP target information.
- Perform DNS-related checks using tools like DNSDumpster and DigWebInterface.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Subdomain Takeover</strong></summary>

- Utilize tools like Can I Take Over XYZ to check for subdomain takeover opportunities.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Passive Reconnaissance</strong></summary>

- Use Google Dorks for reconnaissance with advanced search operators.
- Leverage threat intelligence gathering tools like theHarvester.
- Perform WHOIS Lookup to gather domain registration information.
- Analyze robots.txt for insights into the site's structure.
- Spider the website for URLs using tools like gobuster.
- Conduct DNS Enumeration using tools like dnsrecon.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Active Reconnaissance</strong></summary>

- Conduct advanced port scanning using Nmap.
- Perform service fingerprinting with banner grabbing.
- Utilize network sniffing fingerprinting using Nmap scripts.
- Check for subdomain takeover using tools like subjack.
- Scan the web application using tools like nikto and gobuster.
- Conduct SSL/TLS vulnerability checks with testssl.sh.
- Verify HTTP security headers using gobuster.
</details>
</details>

<details>
<summary style="color: #3498db; font-size: 18px;"><strong>Bug Testing</strong></summary>
<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Injection Vulnerabilities</strong></summary>

- Test for SQL injection vulnerabilities.
- Check for OS command injection vulnerabilities.
- Assess LDAP injection vulnerabilities.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Cross-Site Scripting (XSS)</strong></summary>

- Test for reflected XSS vulnerabilities.
- Check for stored XSS vulnerabilities.
- Assess DOM-based XSS vulnerabilities.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Cross-Site Request Forgery (CSRF)</strong></summary>

- Test for CSRF vulnerabilities.
- Verify the effectiveness of CSRF protection mechanisms.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Security Misconfigurations</strong></summary>

- Check for exposed sensitive information.
- Test for default credentials on administrative interfaces.
- Verify secure configuration of cloud services.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Insecure Direct Object References (IDOR)</strong></summary>

- Test for IDOR vulnerabilities.
- Verify that users cannot access unauthorized resources.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Server-Side Request Forgery (SSRF)</strong></summary>

- Test for SSRF vulnerabilities.
- Verify that the application filters or blocks malicious requests.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>File Upload Security</strong></summary>

- Test for unrestricted file uploads.
- Check for proper validation of file types and content.
- Verify secure storage and access controls for uploaded files.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>XML External Entity (XXE) Injection</strong></summary>

- Test for XXE vulnerabilities in XML parsing.
- Verify that XML inputs are properly validated and sanitized.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Security Headers</strong></summary>

- Check for the presence and effectiveness of security headers.
- Include headers such as Content Security Policy (CSP) and Strict-Transport-Security (HSTS).
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Clickjacking</strong></summary>

- Test for clickjacking vulnerabilities.
- Verify that UI elements cannot be embedded in iframes without proper controls.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Business Logic Testing</strong></summary>

- Test for logical flaws in the application workflow.
- Verify the enforcement of business rules and access controls.
- Assess the impact of parameter manipulation on business processes.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Cryptographic Vulnerabilities</strong></summary>

- Check for weak or deprecated cryptographic algorithms.
- Verify the secure storage and transmission of sensitive information.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>Mobile-specific Vulnerabilities</strong></summary>

- Test for mobile application-specific vulnerabilities.
- Verify the security of APIs used by mobile applications.
- Assess the storage and handling of sensitive information on mobile devices.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>API Security</strong></summary>

- Test the security of APIs for vulnerabilities.
- Verify proper authentication and authorization mechanisms.
- Assess the handling of input data and error messages.
</details>

<details>
<summary style="color: #e74c3c; font-size: 16px;"><strong>IoT-specific Vulnerabilities</strong></summary>

- Test for security vulnerabilities in IoT devices.
- Assess the communication security of IoT devices.
- Verify the security of firmware and update mechanisms.
</details>
</details>

**Feel free to contribute and improve this checklist for the benefit of the community.**

<details>
<summary style="color: #3498db; font-size: 18px;"><strong>Contributors</strong></summary>

- [Sicko]
- [Reconnaissance Command Line Helpful Guide](https://docs.google.com/document/d/1TPPJwzTl8-sqQCLV7dJoKG-0oqDTLdaKcaQUZBA0vmU/edit#heading=h.ab50wugjcygo)
</details>

---

**Sources:**

- [Google Dorking Checklist](https://docs.google.com/document/d/1E64dNgDqQDyXtrj0EPsb4Pi28HXLtvS0buyGsY_78IA/edit)
- [Reconnaissance Command Line Helpful Guide](https://docs.google.com/document/d/1TPPJwzTl8-sqQCLV7dJoKG-0oqDTLdaKcaQUZBA0vmU/edit#heading=h.ab50wugjcygo)
