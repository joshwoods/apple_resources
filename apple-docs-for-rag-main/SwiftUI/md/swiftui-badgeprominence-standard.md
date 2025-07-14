

- SwiftUI
- BadgeProminence
-  standard 

Type Property

# standard

The standard level of prominence for a badge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let standard: BadgeProminence
```

## Discussion

This level of prominence should be used for badges that display a value that suggests user action, such as a count of unread messages or new invitations.

In lists on macOS, this results in a badge label on a grayscale platter; and in lists on iOS, this prominence of badge has no platter.

```
List(mailboxes) { mailbox in
    Text(mailbox.name)
        .badge(mailbox.numberOfUnreadMessages)
}
.badgeProminence(.standard)
```

## See Also

### Getting background prominence

static let increased: BadgeProminence

The highest level of prominence for a badge.

static let decreased: BadgeProminence

The lowest level of prominence for a badge.

