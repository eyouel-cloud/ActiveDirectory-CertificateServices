# Active Directory Certificate Services (AD CS) Lab

This lab walks through setting up a basic internal PKI using AD CS and using it to secure an IIS website with HTTPS.

## Objectives

- Install AD CS and configure a root CA.
- Create a Web Server certificate template.
- Allow enrollment for domain computers or a web server group.
- Deploy IIS on a member server.
- Request a certificate and bind it to an HTTPS site.

## High-Level Steps

1. On a domain-joined server (e.g., `DC01`), install the **Active Directory Certificate Services** role.
2. Configure an Enterprise Root CA.
3. In the Certification Authority console:
   - Duplicate the **Web Server** template.
   - Set permissions for enrollment (e.g., `Domain Computers`, `WebServers` group).
4. On an IIS server:
   - Install the Web Server (IIS) role.
   - Request a certificate from AD CS using the new template.
   - Bind the certificate to the site on port 443.
5. From a domain-joined client, browse to the HTTPS URL and verify the certificate chain.

This lab demonstrates PKI fundamentals and how internal CAs are commonly used to secure web services.
## Author
## Eyouel Melaku ## 
