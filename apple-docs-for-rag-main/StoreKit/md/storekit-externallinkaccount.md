

- StoreKit
-  ExternalLinkAccount 

Enumeration

# ExternalLinkAccount

Enables qualifying apps to link to an external website for account creation or management.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.4+

``` source
enum ExternalLinkAccount
```

## Overview

This functionality is only available to apps with the com.apple.developer.storekit.external-link.account entitlement. For more information, see Distributing “reader” apps with a link to your website.

## Topics

### Linking to external accounts

static var canOpen: Bool

A Boolean value that indicates whether the app can open the external link account.

static func open() async throws

Presents a continuation sheet that enables people to choose whether to open your app’s link to an external website for account creation or management.

## Relationships

### Conforms To

- Sendable

## See Also

### External accounts

com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

