

- SwiftUI
-  MenuActionDismissBehavior 

Structure

# MenuActionDismissBehavior

The set of menu dismissal behavior options.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct MenuActionDismissBehavior
```

## Overview

Configure the menu dismissal behavior for a view hierarchy using the menuActionDismissBehavior(_:) view modifier.

## Topics

### Getting dismiss behaviors

static let automatic: MenuActionDismissBehavior

Use the a dismissal behavior that’s appropriate for the given context.

static let disabled: MenuActionDismissBehavior

Never dismiss the presented menu after performing an action.

static let enabled: MenuActionDismissBehavior

Always dismiss the presented menu after performing an action.

## Relationships

### Conforms To

- Equatable

## See Also

### Configuring menu dismissal

func menuActionDismissBehavior(MenuActionDismissBehavior) -> some View

Tells a menu whether to dismiss after performing an action.

