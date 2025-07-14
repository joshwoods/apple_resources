

- App Store Connect API
- Merchant ID
-  Managing merchant IDs and Payment Processing certificates 

Article

# Managing merchant IDs and Payment Processing certificates

Create and update certificates so your app uses Apple Pay and Wallet.

## Overview

Managing your merchant Identifier (ID) and Payment Processing certificates keeps the Apple Pay service active in your app. To set up your Apple developer account and Xcode to implement Apple Pay in your apps, complete three steps:

- Create a merchant ID.

- Create a Payment Processing certificate. To learn more about certificates for Apple Pay and Wallet, see Configure Apple Pay.

- Enable Apple Pay in Xcode. To learn more see, Setting up Apple Pay Once you set up Apple Pay in your apps, you then can replace Payment Processing certificates as they near their expiration date — 25 months after you create them. To learn more, see Maintaining Your Environment.

### Create a merchant ID

A merchant ID uniquely identifies you to Apple Pay as a merchant who is able to accept payments. A merchant ID never expires, and you can use the same one for multiple apps.

To create a merchant ID, use Create a merchant ID.

Here’s an example payload:

```
"data": {
        "type": "merchantIds",
        "attributes": {
            "identifier": "com.myapp.merchant1",
            "name": "MyMerchantName"
        }
    }
}
```

Note

The value for `identifier` is a unique identifier for your merchant. The value for `name` is a descriptive name for the merchant.

### Create Payment Processing certificate

To create a certificate to use with Apple Pay, use Create a Certificate.

Here’s an example payload:

```
{
  "data": {
    "type": "certificates",
    "attributes": {
        "certificateType": "APPLE_PAY",
        "csrContent" : ""
    },
    "relationships": {
      "merchantId": {
        "data": {
          "type": "merchantIds",
          "id": "1234567890"
        }
      }
    }
  }
}
```

Note

The `id` field in the example payload is a 10-character string that the prior request returns. The `csrContent` is your certificate-signing request.

### Rotate a Payment Processing certificate

Use one of three options to replace a payment-processing certificate nearing its 25-month expiration date. Each option takes into account that you can have more than one payment processing certificate, but only one can be `activated` for use at any time:

Expire and create  
Let the existing Payment Process certificate expire. Then create a new Payment Processing certificate using Create a Certificate. The created certificate automatically has the `activated` key set to `TRUE`.

Create then revoke  
Create a new Payment Processing certificate using Create a Certificate. Revoke the existing certificate nearing expiration by using Revoke a Certificate. The new Payment Processing certificate automatically has the `activated` key set to `TRUE`.

Create and activate  
Create a new Payment Processing certificate using Create a Certificate. Then explicitly “activate” the new certificate using Modify a certificate.

Note

The “Create and activate” option also deactivates the expiring certificate by automatically setting the `activated` key to `FALSE`.

## See Also

### Managing merchant IDs

List merchant IDs

List all merchant Ids for your team.

Read details for a merchant ID

Get information for a merchant ID.

List certificates for a merchant ID

Get a list of all certificates for a specific merchant ID.

Modify merchant IDs

Update a specific merchant ID.

Create a merchant ID

Add a new merchant ID to your team.

Delete a merchant ID

Delete a specific merchant ID.

