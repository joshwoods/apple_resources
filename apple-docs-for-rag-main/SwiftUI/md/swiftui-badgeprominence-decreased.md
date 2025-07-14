

- SwiftUI
- BadgeProminence
-  decreased 

Type Property

# decreased

The lowest level of prominence for a badge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let decreased: BadgeProminence
```

## Discussion

This level or prominence should be used for badges that display a value of passive information that requires no user action, such as total number of messages or content.

In lists on iOS and macOS, this results in badge labels being displayed without any extra decoration. On iOS, this looks the same as `.standard`.

```
List(folders) { folder in
    Text(folder.name)
        .badge(folder.numberOfItems)
}
.badgeProminence(.decreased)
```

## See Also

### Getting background prominence

static let standard: BadgeProminence

The standard level of prominence for a badge.

static let increased: BadgeProminence

The highest level of prominence for a badge.

