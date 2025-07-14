

- WebKit
- WKWebExtension
- WKWebExtension.Action
-  hasUnreadBadgeText 

Instance Property

# hasUnreadBadgeText

A Boolean value indicating whether the badge text is unread.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasUnreadBadgeText: Bool { get set }
```

## Discussion

This property is automatically set to `YES` when badgeText changes and is not empty. If badgeText becomes empty or the popup associated with the action is presented, this property is automatically set to `NO`. Additionally, it should be set to `NO` by the app when the badge has been presented to the user. This property is useful for higher-level notification badges when extensions might be hidden behind an action sheet.

