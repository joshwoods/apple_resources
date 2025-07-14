

- SwiftUI
-  ToolbarCustomizationBehavior 

Structure

# ToolbarCustomizationBehavior

The customization behavior of customizable toolbar content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ToolbarCustomizationBehavior
```

## Overview

Customizable toolbar content support different types of customization behaviors. For example, some customizable content may not be removed by the user. Some content may be placed in a toolbar that supports customization overall, but not for that particular content.

Use this type in conjunction with the customizationBehavior(_:) modifier.

## Topics

### Getting customization behaviors

static var `default`: ToolbarCustomizationBehavior

The default customization behavior.

static var disabled: ToolbarCustomizationBehavior

The disabled customization behavior.

static var reorderable: ToolbarCustomizationBehavior

The reorderable customization behavior.

## Relationships

### Conforms To

- Sendable

## See Also

### Populating a customizable toolbar

func toolbar&lt;Content>(id: String, content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items, allowing for user customization.

protocol CustomizableToolbarContent

Conforming types represent items that can be placed in various locations in a customizable toolbar.

struct ToolbarCustomizationOptions

Options that influence the default customization behavior of customizable toolbar content.

