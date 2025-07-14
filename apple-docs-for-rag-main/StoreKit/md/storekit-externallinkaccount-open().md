

- StoreKit
- ExternalLinkAccount
-  open() 

Type Method

# open()

Presents a continuation sheet that enables people to choose whether to open your app’s link to an external website for account creation or management.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.4+

``` source
static func open() async throws
```

## Discussion

Call this method in response to deliberate user interaction, for example, tapping a button. Call canOpen to determine whether to display a button or other user-interface control. If canOpen is `false`, this method always throws a StoreKitError instance.

## See Also

### Linking to external accounts

static var canOpen: Bool

A Boolean value that indicates whether the app can open the external link account.

