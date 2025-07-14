

- SwiftUI
-  AccessibilityQuickActionStyle 

Protocol

# AccessibilityQuickActionStyle

A type that describes the presentation style of an accessibility quick action.

watchOS 9.0+

``` source
protocol AccessibilityQuickActionStyle
```

## Topics

### Getting built-in menu styles

static var outline: AccessibilityQuickActionOutlineStyle

A presentation style that animates an outline around the view when the accessibility quick action is active.

static var prompt: AccessibilityQuickActionPromptStyle

A presentation style that displays a prompt to the user when the accessibility quick action is active.

### Supporting types

struct AccessibilityQuickActionOutlineStyle

A presentation style that displays a prompt to the user when the accessibility quick action is active.

struct AccessibilityQuickActionPromptStyle

A presentation style that displays a prompt to the user when the accessibility quick action is active.

## Relationships

### Conforming Types

- AccessibilityQuickActionOutlineStyle
- AccessibilityQuickActionPromptStyle

## See Also

### Offering Quick Actions to people

func accessibilityQuickAction&lt;Style, Content>(style: Style, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

func accessibilityQuickAction&lt;Style, Content>(style: Style, isActive: Binding&lt;Bool>, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

