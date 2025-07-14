

- UIKit
- UICalendarView
- UICalendarView.Decoration
-  default(color:size:) 

Type Method

# default(color:size:)

Creates a default calendar view decoration with a filled circle image, using the color and size you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
static func `default`(
    color: UIColor? = nil,
    size: UICalendarView.DecorationSize = .medium
) -> UICalendarView.Decoration
```

## Parameters 

`color`  

A color for the decoration.

`size`  

A relative size for the decoration.

## Return Value

A calendar view decoration.

## See Also

### Creating a Default Decoration View

init()

Creates a default calendar view decoration with a filled circle image, using the system fill color and medium size.

