

- StoreKit
-  External link account 

API Collection

# External link account

Enable qualifying apps to link to an external website for account creation or management.

## Overview

If you develop a qualifying app, you can complete a request for an entitlement that allows you to link to an external website for account creation or management. For more information about whether your app qualifies and how to request an entitlement, see Distributing “reader” apps with a link to your website.

If your account has the com.apple.developer.storekit.external-link.account entitlement, implement the following to link to an external website for account creation and management:

- Configure the SKExternalLinkAccount property list key.

- Use the ExternalLinkAccount type’s canOpen property and open() method.

Note

In a compatible iPad or iPhone app running in visionOS, on a Mac with Apple silicon, or on a Mac app built with Mac Catalyst, the External Link Account APIs throw an error or return `false`.

## Topics

### External accounts

com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

enum ExternalLinkAccount

Enables qualifying apps to link to an external website for account creation or management.

