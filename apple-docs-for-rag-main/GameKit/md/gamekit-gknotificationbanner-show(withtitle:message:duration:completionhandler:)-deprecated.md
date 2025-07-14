

- GameKit
- GKNotificationBanner
-  show(withTitle:message:duration:completionHandler:) Deprecated

Type Method

# show(withTitle:message:duration:completionHandler:)

Displays a banner to the player for a specified period of time.

iOS 5.0–16.1DeprecatediPadOS 5.0–16.1DeprecatedMac Catalyst 13.1–16.1DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func show(
    withTitle title: String?,
    message: String?,
    duration: TimeInterval,
    completionHandler: (() -> Void)? = nil
)
```

``` source
class func show(
    withTitle title: String?,
    message: String?,
    duration: TimeInterval
) async
```

Deprecated

Use UNNotificationRequest or provide a custom interface instead.

## Parameters 

`title`  

The title of the banner.

`message`  

The message on the banner.

`duration`  

The amount of time that GameKit should dispay the banner to the player.

`completionHandler`  

The block that GameKit calls when the player or GameKit dismisses the banner.

## See Also

### Displaying the Banner

class func show(withTitle: String?, message: String?, completionHandler: (() -> Void)?)

Displays a banner with a title and message to the player.

Deprecated

