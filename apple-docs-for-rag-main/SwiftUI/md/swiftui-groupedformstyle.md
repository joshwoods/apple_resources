

- SwiftUI
-  GroupedFormStyle 

Structure

# GroupedFormStyle

A form style with grouped rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct GroupedFormStyle
```

## Overview

Rows in this form style have leading aligned labels and trailing aligned controls within visually grouped sections.

Use the grouped static variable to create this style:

```
Form {
   ...
}
.formStyle(.grouped)
```

## Topics

### Creating the form style

init()

Creates a form style with scrolling, grouped rows.

## Relationships

### Conforms To

- FormStyle

## See Also

### Supporting types

struct AutomaticFormStyle

The default form style.

struct ColumnsFormStyle

A non-scrolling form style with a trailing aligned column of labels next to a leading aligned column of values.

