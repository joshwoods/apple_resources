

- SwiftUI
- MenuActionDismissBehavior
-  automatic 

Type Property

# automatic

Use the a dismissal behavior that’s appropriate for the given context.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static let automatic: MenuActionDismissBehavior
```

## Discussion

In most cases, the default behavior is enabled. There are some cases, like Stepper, that use disabled by default.

## See Also

### Getting dismiss behaviors

static let disabled: MenuActionDismissBehavior

Never dismiss the presented menu after performing an action.

static let enabled: MenuActionDismissBehavior

Always dismiss the presented menu after performing an action.

