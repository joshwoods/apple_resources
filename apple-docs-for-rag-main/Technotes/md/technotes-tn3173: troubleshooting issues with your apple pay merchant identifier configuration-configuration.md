

- Technotes
-  TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration 

Article

# TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

## Overview

This technote covers debugging common issues with your merchant identifier (merchant ID) and certificates required for Apple Pay. For more information about configuring your merchant ID and certificates required for Apple Pay, see Configuring Your Environment.

This technote does not cover configuring Apple Pay on the Web when adopted via a platform integrator such as a third party e-commerce platform or payment service provider (PSP)— for instance, if you don’t have access to your own Apple Developer account. If you are experiencing issues with onboarding via your e-commerce platform or PSP, talk to these vendors directly.

## Certificate Signing Request formatting issues

When creating a merchant identity certificate or payment processing certificate, you upload a certificate signing request (CSR) in a specific format.

If you receive an error stating the CSR algorithm/size is incorrect, please check that you have created the key-pair and CSR in the correct format for each of the specific certificates. As an example, consider the following error:

```
"CSR algorithm/size incorrect. Expected: RSA(2048)"
```

The expected algorithm/size for each certificate is as follows:

- **Merchant identity certificate:** Use RSA (2048-bit).

- **Payment processing certificate:**

  - For processing payments in China mainland, use RSA (2048-bit).

  - For processing payments in all other regions, use ECC (256-bit).

For more information about generating CSRs for Apple Pay payment processing certificates, see Create a certificate signing request.

## Certificate validation issues

If you have multiple PSPs, ensure your CSR is uploaded to the corresponding PSP for the merchant. Mismatching CSRs causes validation issues. For example, for multiple merchant configurations:

- **Match:** Merchant identity certificate \#1 is uploaded to PSP \#1

- **Mismatch:** Merchant identity certificate \#1 is uploaded to PSP \#2

In addition, for a single merchant process for both RSA and ECC certificates:

- **Match:** Merchant identity certificate using RSA is uploaded to PSP for RSA.

- **Mismatch:** Merchant identity certificate using ECC uploaded to PSP for ECC.

## Domain verification issues

Domain verification can fail for many reasons. Here are some common issues and suggestions on how to address them:

- The Apple domain verification server can’t reach your public server.

- The Apple domain verification server does not trust your server’s TLS implementation, cypher suites, or certificates.

- Your domain is behind a proxy or in a private network.

- Your domain verification file is served via a redirect, is invalid or expired, or is associated with a different domain.

For more information about merchant domain validation, see Setting Up Your Server.

### Apple cannot reach your server

When the domain verification request fails, it may be unclear why the failure occurred. To debug this scenario:

- Review your server’s access logs for any errors or failed connections.

  - Temporarily set your server logs to be verbose, if your default log levels don’t identify an issue.

- Make sure that the domain verification request is reaching your server.

  - If the request is not reaching the server, then there is an issue with Apple’s domain verification server reaching your server.

  - If the request is reaching your server, and it is not a TLS issue, then your server-side logs should provide more insight into the underlying cause of the connection failures to the Apple servers.

### Apple does not trust your server

Even though your server supports TLS 1.2 and later, uses the correct Apple IP ranges in your allowlists, and leverages the correct cypher suites, you can still experience domain verification failures.  
This typically indicates that you have an untrusted root certificate for the current Apple operating system. For a complete list of trusted root certificates, see Available trusted root certificates for Apple operating systems.

### Your domain is behind a proxy or in a private network

A network proxy or load balancer might be routing traffic incorrectly. Apple’s domain verification server not only validates your merchant domain verification file, but also reads client-specific information about your TLS certificate. When this request flows through a proxy it will gather incorrect information about your domain’s certificate because of the proxy. Another issue occurs when there is a proxy that your server communicates with and Apple’s domain verification server cannot directly reach the server where the domain is hosted. In this case, the proxy may need to be removed.

Domain verification issues for a server sitting behind a load balancer are uncommon but can happen when the load balancer is routing traffic incorrectly. If you think this is the case for network, double-check the routing algorithm on your load balancer to ensure that traffic always makes it to your server.

Lastly, if your domain is on a private network and needs to be verified, make sure that Apple’s domain verification server IP addresses are allowed in your network’s bi-directional firewall rules. To learn more about these IP address ranges, see Setting Up Your Server.

### Your domain verification file is served via a redirect

To verify the domain, the Apple domain verification server will make a request to the specific file path and will expect the contents of the domain verification file to be returned in the response body, alongside a `200 OK` HTTP status.

When the domain verification file is made available via a redirect, the domain verification server is unable to verify the domain as Apple cannot confirm the response has come from the same domain that was registered. You should remove any redirects and serve the response directly from the server and domain that received the request.

### Your domain verification file is invalid or expired

The domain verification file is only valid for seven (7) days after generation. If you attempt to verify the domain after this time, the process will not complete successfully and a new file should be generated and verified within another seven (7) days.

It is also worth noting that only the most recently generated file for each domain is considered valid. Each time you generate a new domain verification file it will invalidate all previously generated files. Ensure that you also have the most recent file.

### Your domain verification file is associated to a different domain

The domain verification file generated is specific to the exact domain that you register for your Apple Developer account. This means the value registered must match exactly to the domain where the verification file is served from—including any subdomains, as well as the `www.` subdomain.

If your domain is available both with and without the `www.` subdomain, it is recommended that you register and verify both variants to ensure all users can successfully access Apple Pay, regardless of the domain they used to access at your website.

Note

If your website uses multiple subdomains (such as `example.com`, `www.example.com`, and `shop.example.com`), each requires its own entry as a registered merchant domain, and each must serve its own domain verification file.

If you attempt to verify your domain with a file associated with a different domain, you will not be able to successfully complete verification. So ensure you use the file specific to the domain you have registered.

### Your domain does not automatically re-verify

Apple Pay periodically re-verifies your domain based on the expiration date of your SSL certificate. In most cases, however, there are a few things that can affect the success of this automatic  
re-verification process.

The Apple domain verification server attempts domain re-verification thirty (30) days before your SSL certificate expires by making a request to the same path used for the original verification process. You don’t need to update or replace the file—the domain verification server expects a response with a `200 OK` HTTP status at this file path. In addition, the domain verification server makes a request to your root domain (e.g. `subdomain.example.com`) and expects a response with a `200 OK` HTTP status.

If the domain verification server is unable to re-verify your domain, it will re-attempt verification fifteen (15) days before, and then once again seven (7) days before, the SSL certificate expires. If automatic re-verification fails, you may need to manually re-verify the domain again by downloading and placing a new verification file on your server.

Please confirm the following when automatic re-verification fails:

- The domain verification file path returns a `200 OK` HTTP status when a verification request is made.

- The root domain returns a `200 OK` HTTP status when a verification request is made.

- Your SSL certificate has been replaced/updated with a new expiry.

- The SSL certificate chain of trust has not changed. The domain expiry extension operation relies on consistency of the domain certificate chain. Therefore, the certificate chain returned by the domain must match the version the domain verification server cached from the original certificate.

## Revision History

- **2024-06-11** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

