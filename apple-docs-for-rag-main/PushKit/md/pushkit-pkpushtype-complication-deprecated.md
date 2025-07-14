

- PushKit
- PKPushType
-  complication Deprecated

Type Property

# complication

A push type for watchOS complications.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 9.0–13.0DeprecatedwatchOS 6.0+

``` source
static let complication: PKPushType
```

Deprecated

Complication pushes are supported directly on watchOS now, so this should no longer be used on iOS.

## Discussion

Use this type of notification to deliver updated data related for your watchOS app’s complication. The watchOS app’s complication must be active on the user’s current clock face. If it is not, the system does not deliver pushes of this type. For watchOS 6 and later, send the push notification directly to Apple Watch. For watchOS 5 and earlier, you must send it to the iOS companion instead.

The time your watchOS app spends processing these push notifications counts against the budget allotted to your complication for updating itself. Don’t start any long-running tasks when processing the notification payload. In fact, it is recommended that you include all needed data in the payload so that your app can process that data quickly.

The system limits you to 50 push notifications per day. If you exceed the limit, subsequent pushes are not delivered.

## See Also

### Notification Types

static let fileProvider: PKPushType

A push type for file provider updates.

static let voIP: PKPushType

A push type for Voice-over-IP (VoIP) call invitations.

