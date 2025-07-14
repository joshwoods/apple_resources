

- Apple Pay Web Merchant Registration API
-  Preparing Merchant Domains for Verification 

Article

# Preparing Merchant Domains for Verification

Host a domain verification file on each domain before requesting registration.

## Overview

Before making a Register Merchant request, you must prepare each domain included in the request for verification. When Apple grants you access to use this API, Apple sends you a domain-verification file for each merchant ID you registered. Use these verification files for your merchant registrations.

Important

The domain-verification files you receive when you’re granted access to the API are distinct from the file available in the Apple Merchant ID section of the Apple Developer portal. Only use the verification files you receive.

Host your domain-verification file at the following path for each domain you’re registering:

`https://[DOMAIN_NAME]/.well-known/apple-developer-merchantid-domain-association`

The domain-verification file must be in place before you invoke the Register Merchant API. Be sure to use the domain-verification file associated with the merchant ID that you provide in the `encryptTo` field.

Apple Pay servers don’t require domain verification in the sandbox environment. You receive domain-verfication files for merchant IDs that have access to production servers only.

## See Also

### Web Merchant Registration

Register Merchant

Register a merchant and its corresponding set of fully qualified domains.

object RegisterMerchantRequest

The request body you use to register merchants.

