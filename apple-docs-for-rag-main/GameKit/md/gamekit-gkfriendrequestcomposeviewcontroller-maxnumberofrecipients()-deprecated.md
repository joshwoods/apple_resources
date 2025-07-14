

- GameKit
- GKFriendRequestComposeViewController
-  maxNumberOfRecipients() Deprecated

Type Method

# maxNumberOfRecipients()

Returns the maximum number of recipients permitted in a single request.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class func maxNumberOfRecipients() -> Int
```

Deprecated

No longer supported.

## Return Value

The maximum number of recipients.

## Discussion

If you add more recipients than the value returned from this method, GameKit throws an exception.

