

- SwiftUI
-  ToolbarCustomizationOptions 

Structure

# ToolbarCustomizationOptions

Options that influence the default customization behavior of customizable toolbar content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ToolbarCustomizationOptions
```

## Overview

Use this type in conjunction with the defaultCustomization(_:options:) modifier.

## Topics

### Getting customization options

static var alwaysAvailable: ToolbarCustomizationOptions

Configures default customizable toolbar content to always be present in the toolbar.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Populating a customizable toolbar

func toolbar&lt;Content>(id: String, content: () -> Content) -> some View

Populates the toolbar or navigation bar with the specified items, allowing for user customization.

protocol CustomizableToolbarContent

Conforming types represent items that can be placed in various locations in a customizable toolbar.

struct ToolbarCustomizationBehavior

The customization behavior of customizable toolbar content.

