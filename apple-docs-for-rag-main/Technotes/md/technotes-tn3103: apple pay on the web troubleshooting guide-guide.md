

- Technotes
-  TN3103: Apple Pay on the Web troubleshooting guide 

Article

# TN3103: Apple Pay on the Web troubleshooting guide

Troubleshooting guide for implementing Apple Pay on the Web.

## Overview

This document is intended to be used as a general guide to debugging common issues with Apple Pay on the Web. Note that this document does not cover third-party tooling or integrations. If you are experiencing issues with third-party code, libraries, or server side configurations, you will need to talk to these vendors directly. This document assumes that you are building Apple Pay on the Web from your own website and then integrating with a third-party Payment Service Provider.

## Creating merchant assets

Your Developer Account registers a Merchant by creating a new Merchant Identifier (Merchant ID) in Certificates, Identifiers & Profiles. A Merchant ID is the unique identifier for your Merchant Domain, Merchant Identity Certificate, Payment Processing Certificate, and Merchant Assets. A Merchant ID will be in reverse-DNS format: `merchant.com.testbed.applepay`.

Note

If you are working with a Payment Service Provider who can give you access to Apple Pay without an Apple Developer Account, the process outlined below will be different and you should contact the the Payment Service Provider for additional help on configuring your Merchant Assets.

After you have created your Merchant Identifier you will need to create a Payment Processing Certificate using a 256-bit ECC key pair. However, if you are using a third-party Payment Service Provider, they may provide this certificate for you. If so, skip to Step 2 below.

### Create a payment processing identity

1.  On your Mac, launch Keychain Access to create a certificate signing request (CSR).

2.  Upload this CSR to the Merchant Configuration page to generate a Payment Processing Certificate.

3.  Create a Payment Processing Identity (p12 / key and cert) by downloading the generated Payment Processing Certificate and installing it into the Keychain on the same Mac used to create the initial CSR. If you created the CSR outside of a Mac then the key and certificate will need to be stored on the device the CSR was created. **Important**: Do not lose this Payment Processing Identity, because it will be used by your Payment Processor.

Note

The process described here details a situation where you, as the Developer, are setting up the Merchant Assets. It could also be the case that your Payment Service Provider creates the CSR and gives it to you, the Merchant, to upload to the Merchant ID Configuration page to generate a Payment Certificate. The benefit of this workflow is you would not need to export your Payment Processing Identity from your Keychain to provide it to the Payment Processor, they would already have the required private key from the CSR that they had previously generated.

### Create a merchant identity certificate

In the Merchant ID Configuration page under your Merchant Identifier, you will need to create a Merchant Identity Certificate in the same place you created the Payment Processing Certificate.

1.  On your Mac, launch Keychain Access to create a certificate signing request (CSR) with an RSA 2048-bit RSA key pair.

2.  Upload this CSR to the Merchant Configuration page to generate a Merchant Identity Certificate.

3.  Create a Merchant Identity (p12 / key and cert) by downloading the generated Payment Merchant Certificate and installing it into the Keychain on the same Mac used to create the initial CSR. If you created the CSR outside of a Mac then the key and certificate will need to be stored on the device the CSR was created.

Note

A CSR does not have to be created in the Keychain of a macOS computer. A CSR can technically be created from an external source such as a server, another workstation, or from your Payment Service Provider, with a tool like OpenSSL.

The important thing to remember is that when a CSR is created, so is a private key. After uploading the CSR to the Apple Developer Portal and receiving a certificate, you will need to store the certificate and the private key in a secure location so that a PKCS#12 (or p12) can be created from both the private key and certificate. The Keychain on macOS does this for you and so you do not have to worry about it, but if using an external tool, you will need to do this by hand. The creation of a p12 from a private key and certificate is what makes up a digital identity, and this is what is used to authenticate your team as a Merchant to the Apple Pay servers. For example, the creation of a Merchant Identity in the form of a p12, or a stacked PEM, contains your private key and Merchant Certificate. These assets that are tied to your Merchant account are then used to perform client authentication when requesting a payment session from the Apple Pay servers.

It is important that the digital identity in this context be correctly formatted and stored in a secure location if created outside of macOS. If you do end up creating this identity outside macOS, you will be responsible for converting certificate and private key into a format that can be used for Merchant Authentication.  
The Payment Processing Identity will be used to decrypt your payment tokens by your Payment Processor.

### Registering a merchant domain

You will need to add a Merchant domain to your Merchant Identifier so that your domain can process payments. You will need to register each domain that you plan to process payments from. For example, if you plan to process payments on `example.com` and `test.example.com` you will need to register and verify each domain. Note, if you plan to process payments for `example.com`, and you will actually be using `www.example.com`, make sure to include the fully qualified domain name (FQDN) in the registration process.  
An FQDN in this context would be `www.example.com`.

## Domain verification

Once your domain is configured in the Merchant ID Configuration page for `example.com`, you will be asked to verify your domain with a `apple-developer-merchantid-domain-association.txt` file. On your server, download the file and place it in the `.well-known` location:

```
https://example.com/.well-known/apple-developer-merchantid-domain-association.txt
```

This file above will need to be placed at the root level of your server.

Important

The domain verification file expires after **7 days**, so if you are not able to verify your domain after 7 days you will need to regenerate this file and replace it on your server.

To perform domain verification, click the Verify button in the Merchant ID Configuration page to verify the domain. If all goes well, your domain should be verified and show up as “Verified” in the Merchant ID Configuration page. If you experience issues, please read further to resolve common reasons domain verification fails.

## Common reasons domain verification fails

Domain verification can fail for many reasons. Here are a few of the most common reasons:

### TLS handshake cannot be established

There are many reasons why a TLS handshake can fail during the domain verification process. For example, your server may be misconfigured in the following ways:

- The server does not support TLS 1.2 or above

- The server does not support one of the specified cipher suites for Apple Pay

- The server is using an invalid TLS certificate

#### Supporting TLS 1.2 or above

Servers supporting Apple Pay on the Web need to being using TLS 1.2 or above. Servers also need to be accessible by the domain verification client and not be sitting behind a proxy.

#### Validating usage of a TLS cipher suite

Servers negotiating TLS connections for Apple Pay on the Web need to use one of the supported cipher suites described in Setting up your Server. To debug which cipher suites is being negotiated between Apple’s domain verification client and your server, take a packet trace and take a look at the the cipher suites being offered by Apple’s domain verification client in the `Client Hello` packet. If all goes well, you will be able to see one of the supported cipher suites being selected by your server in the `Server Hello` packet being sent back to the client. If there is an issue in the cipher suite negotiation then there will typically be a failure after the `Client Hello` packet.

#### Validating TLS 1.2 certificates

Make sure that you are using a valid TLS certificate. For example, make sure that this certificate is setup with a proper chain of trust and also adheres to Apple’s Certificate Transparency policy for Safari. You can double check this with a packet trace. Make sure the leaf certificate being used on your domain follows a correct chain of trust through the intermediate certificates to the root certificate.

### The Apple Developer Portal cannot reach your server

One common problem is that the domain verification request seems to error out, but there is no apparent reason why this is happening. To debug this, try reviewing your server’s access logs, or try setting your server application logs to be as verbose as possible. Next, make sure that the domain verification request is reaching your server. If the request is not reaching the server then you know there is an issue with Apple’s domain verification client reaching your server. If the request is reaching your server, and it is not a TLS issue, then your server side logs should provide more insight here on where the issue is taking place.

### Your domain sits behind a proxy or in a private network

One common issue is that a domain sits behind a network proxy or a load balancer that is not correctly routing traffic. In the case of the proxy, this is problematic because Apple’s domain verification client is trying to validate your domain verification file, but also read client specific information about your TLS certificate. When this request flows through a proxy it will pickup incorrect information about your domain’s certificate because of the proxy.  
The proxy will need to be removed.

Domain verification issues for a server sitting behind a load balancer are not common but can happen when the load balancer is routing traffic incorrectly. If you think this is the case for network, double check the routing algorithm on your load balancer to ensure that traffic always makes it to your server.

Lastly, if you domain sits inside of a private network and needs to be verified, make sure that Apple’s domain verification client IP addresses are allowed in your network’s firewall. See more on these IP Ranges here.

## Building your client application

Building the client application is done with either ApplePay JS or the Payment Request API. This document will use examples from ApplePay JS. There are many paths you can take here, but as a prerequisite, you need to first make sure that the browser supports Apple Pay. For more details on this see Checking for Apple Pay Availability.

After your application has verified that the browser supports Apple Pay, then it is time to build out the payment workflow. For a complete step by step example of how this is done, see the Apple Pay on the Web Interactive Demo. This demo includes sample code that outlines each step in the payment workflow, and can come in handy when determining how to build your application.

When building out your payment workflow you should consider how you will build out your payment request. For example, in the payment request below, only the required information needed to completion the shopping cart transaction is added, and this is the recommendation.

```
```

For example, if you are charging one flat fee for shipping, or are not charging for shipping at all, then the following payment request would be sufficient. However, if you need to calculate transaction totals based on location or address then you have two options. The first is to gather this shipping information as part of your payment workflow before the payment request is created. That way you have this information up front before the payment workflow. The second option is to pass in information for `requiredShippingContactFields` into your payment request:

```
```

Using the `requiredShippingContactFields` field tells the Apple Pay SDK that you would like to receive redacted shipping and contact information to calculate shipping and further fees on the transaction. These fields will show up in the `onshippingcontactselected` with just enough information to calculate shipping fees.

```
```

After the transaction is authorized you will receive the complete shipping information.

## Merchant validation

After the payment request is created your application will need to go through the Merchant Validation process to authenticate itself as a valid Merchant to process a transaction. Upon successful authentication, your server will receive a payment session to submit with your payment request to the Apple Pay SDK. This process is where most Apple Pay on the Web issues take place because there are a lot of moving parts. Here is an overview of that process as well as suggestions on how to resolve common errors in this workflow:

1.  Call your server with the URL that your client side application received in validationURL. In this step your JavaScript client application will send an HTTPS request to your server side application passing it the validationURL.

2.  Your server side application will receive the HTTPS request from step one, and use the validationURL to create a POST request to obtain a payment session from the server to Apple’s servers. This is where your application uses the Merchant Identity Certificate to identify itself as a valid Merchant to the Apple Pay Servers. **DO NOT** make this request from your client side JavaScript application as it will expose your private key. Make sure this request utilizes the correct format of your p12/PEM to perform client authentication with the Apple Pay servers. If you receive a TLS or SSL failure while making this request then examine the format of the p12/PEM in this payment session request.

3.  Once the Apple Pay server has a payment session it should respond to your server with this session and your client application should pass the session into `completeMerchantValidation(paymentSession);`.

Step two above is where a lot of issues take place. To validate that your server side APIs are not causing an issue, you can test a payment session request using CURL. Assuming that your Merchant Identity Certificate is in your Keychain, export that as a p12 and extract the certificate/key in PEM format.

```
$ openssl pkcs12 -in Certificates.p12 -out apple-pay-cert.pem -nodes -clcerts

```

Then use the CURL command to request a payment session by going around your server.  
If this works, then you know you have a server side API issue.

```
$ curl -gv --data '{"merchantIdentifier":"merchant.com.testbed.applepay", "initiativeContext":"example.com", "initiative":"web", "displayName":"Apple Pay Testbed"}' --cert /path/to/pem/apple-pay-cert.pem https://apple-pay-gateway.apple.com/paymentservices/paymentSession
```

```
```

A successful response here will contain a valid JSON payload with a valid payment session tied to your Merchant ID.

### Payment services exception

If you send a request to the Apple Pay servers to get a Payment Session, and come back with a 400 server response error, the first thing you will want to do is check that your request was formatted correctly. A 400 server response means “Bad Request.” If the request looks fine, then you will want to double check the Merchant ID and the Merchant Identity Certificate that are used on the request. Consider this error:

```
```

Now, this looks hard to read, but to debug this you need to check the `merchantId=` value against a `sha256` hash of the Merchant ID to see if they match. Looking at the hash of my Merchant ID for `merchant.com.testbed.applepay`:

```
echo -n "merchant.com.testbed.applepay" | shasum -a 256
12953b72a8db15cf4a079b49a87ddd5eed1b0ba2eb249c7907265a7b04cff6ce 
```

It looks like something went wrong with the Merchant ID that was used in this request. In this case go back and check the Merchant ID used in the payment session request.

### completeMerchantValidation fails

If you pass a valid payment session into `completeMerchantValidation` and receive an error, there are a few things you can try:

1.  Isolate the issue to a device that is being used for Sandbox testing. For example, make sure you only have a Sandbox test user signed into a device and that you are using the device only for a Sandbox test account. Do not mix production and Sandbox cards and accounts. Create a Sandbox Tester Account.

2.  Make sure the test device is properly authenticating the transaction with Face ID, Touch ID, or watchOS confirmation.

3.  If you continue to have trouble, and can reproduce this issue on macOS, try logging the events from `passd` when the issue is reproduced on macOS with Safari. For example, on macOS, open two terminal windows and run each of these commands in separate Terminal windows:

```
$ log stream --level debug --predicate 'process == "passd"'
$ log stream --level debug --predicate 'subsystem == "com.apple.passkit”'
```

Then reproduce your issue in Safari on macOS. Typically you will see logs that end up like this from these daemons:

```
com.apple.PassKit.PaymentAuthorizationUIExtension: (PassKitCore) [com.apple.passkit:Payment] 
Evaluating merchant session using PROD trust policy.

com.apple.PassKit.PaymentAuthorizationUIExtension: (PassKitCore) [com.apple.passkit:Payment] 
Application failed to provide a valid merchant session. We can't proceed to authorize the transaction.
```

There are a few different reasons these errors can happen:

- A request for a payment session contains a domain other than what is being tested on. For example, testing on `www.example.com` and the request a payment session request is being sent for `staging.example.com`.

- A Merchant Session is considered to have a bad signature because of issues with a Merchant Identity Certificate or Merchant Domain.

- You have not authorized your payment with watchOS, macOS, or iOS.

## Decrypting the payment token

Once you have completed the payment workflow you will need to pass the payment token to your Payment Processor. This is where your Payment Processing Identity comes into play. Your Payment Processor will need your Payment Processing Identity to decrypt the payment token that was encrypted with the public key of your Payment Processing Certificate.

If you attempt to decrypt a payment token and receive something other than a parseable JSON output then the most common reason for this issue is that you have a key mis-match. For example, a payment token is trying to be decrypted with a private key that does not match the public key that the token was encrypted with. When the payment token is encrypted, it is encrypted with Payment Processing Certificate’s public key. This public key should be embedded in the private key as well. If you are able to extract the public key from the private key and compare a sha256 hash of each key, they should match. If the public key hashes do not match then the Payment Processor has the wrong private key. To extract the public key from the private key you should be able to use a tool like OpenSSL to do so.

For a complete overview of how to decrypt the Apple Pay Payment token and how the payment token is structured, please see the Payment Token Format documentation here.

## Revision History

- **2022-05-24** Made minor editorial changes.

- **2022-03-29** Made minor editorial changes.

- **2022-02-08** Republished as TN3103.

- **2021-09-13** First published as “Apply Pay on the Web Debugging Guide” on the Apple Developer Forums.

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

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

