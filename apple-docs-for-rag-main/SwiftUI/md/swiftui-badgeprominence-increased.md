

- SwiftUI
- BadgeProminence
-  increased 

Type Property

# increased

The highest level of prominence for a badge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let increased: BadgeProminence
```

## Discussion

This level of prominence should be used for badges that display a value that requires user action, such as number of updates or account errors.

In lists on iOS and macOS, this results in badge labels being displayed on a red platter.

```
ForEach(accounts) { account in
    Text(account.userName)
        .badge(account.setupErrors)
        .badgeProminence(.increased)
}
```

## See Also

### Getting background prominence

static let standard: BadgeProminence

The standard level of prominence for a badge.

static let decreased: BadgeProminence

The lowest level of prominence for a badge.

