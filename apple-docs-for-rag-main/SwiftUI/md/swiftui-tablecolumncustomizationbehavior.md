

- SwiftUI
-  TableColumnCustomizationBehavior 

Structure

# TableColumnCustomizationBehavior

A set of customization behaviors of a column that a table can offer to a user.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct TableColumnCustomizationBehavior
```

## Overview

This is used as a value provided to disabledCustomizationBehavior(_:).

Setting any of these values as the `disabledCustomizationBehavior(_:)` doesn’t have any effect on iOS.

## Topics

### Getting the customization behavior

static var all: TableColumnCustomizationBehavior

All customization behaviors.

static let reorder: TableColumnCustomizationBehavior

A behavior that allows the column to be reordered by the user.

static let resize: TableColumnCustomizationBehavior

A behavior that allows the column to be resized by the user.

static let visibility: TableColumnCustomizationBehavior

A behavior that allows the column to be hidden or revealed by the user.

### Creating a behavior

init()

Creates an empty customization behavior, representing no customization

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Sendable
- SetAlgebra

## See Also

### Customizing columns

func tableColumnHeaders(Visibility) -> some View

Controls the visibility of a `Table`’s column header views.

struct TableColumnCustomization

A representation of the state of the columns in a table.

