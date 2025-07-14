

- Apple Pay on the Web
-  Configuring Your Environment 

Article

# Configuring Your Environment

Create your Apple Pay merchant ID and certificates, and verify your domain.

## Overview

To support Apple Pay on your website, you must complete the setup steps in your developer account. The steps include registering a merchant ID, creating two certificates, and verifying your domain. Completing the setup enables you to use either or both web APIs: Apple Pay JS API or Payment Request API.

Note

Incorporating Apple Pay on your website is subject to the Apple Pay Acceptable Use Guidelines. You must have an Apple Developer Account to complete the setup, and log in with a Team Agent or Admin role.

### Configure Merchant ID and Certificates

Follow the instructions in Configure Apple Pay on the Web. They guide you to create the following:

- **Merchant ID**. An identifier you register with Apple that uniquely identifies your business as a merchant able to accept payments. This ID never expires, and you can use it in multiple websites and iOS apps. See Create a merchant identifier for the setup steps.

- **Payment processing certificate**. A certificate associated with your merchant ID, used to secure transaction data. Apple Pay servers use the certificate’s public key to encrypt payment data. You, or your payment service provider, use the private key to decrypt data to process payments. See Create a payment processing certificate for the setup steps.

- **Merchant identity certificate**. A Transport Layer Security (TLS) certificate associated with your merchant ID, used to authenticate your sessions with the Apple Pay servers. The merchant identity certificate is only required for Apple Pay on the web; it isn’t needed for apps. See Create a merchant identity certificate for the setup steps.

While your merchant ID never expires, the payment processing certificate, merchant identity certificate, and domain verification do expire. See Maintaining Your Environment for more information.

Tip

You can use the same merchant ID and payment processing certificate in iOS and watchOS apps. If you’re developing apps, enable Apple Pay in Xcode as a last step. See Setting up Apple Pay for more information.

### Register and Verify Your Domain

You must register and verify all top-level domains and subdomains where you’ll display the Apple Pay button. Apple Pay associates domains with your Apple Developer Team ID. As a result:

- You can register multiple domains under a single merchant ID.

- You can register the same domains under multiple merchant IDs.

- You can’t register the same domain with a different Team ID.

Domains can’t be behind a proxy or redirect, and must be accessible to the Apple servers listed in Setting Up Your Server.

To register and verify your domain, log in to your Apple Developer account as an Account Holder or Admin. See Register a merchant domain and Verify a merchant domain for the setup steps.

### Use the Merchant ID in Multiple Environments

It’s up to you to determine how many merchant IDs you need. Most merchants need only one for all environments: in multiple websites, iOS or watchOS apps, across test environments, and production environments.

However, you can create more than one merchant ID if you wish. Be sure to use the payment processing and merchant identity certificates created for the specific merchant ID. The certificates are valid only with their corresponding merchant ID.

## See Also

### Apple Pay setup

Setting Up Your Server

Set up your server for secure communications with Apple Pay.

Maintaining Your Environment

Prevent interruptions in your Apple Pay service by keeping certificates and domain verification current.

