

- UIKit
- UICalendarView
- UICalendarView.Decoration
-  image(\_:color:size:) 

Type Method

# image(\_:color:size:)

Creates a new calendar view decoration with the image, color, and size that you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
static func image(
    _ image: UIImage?,
    color: UIColor? = nil,
    size: UICalendarView.DecorationSize = .medium
) -> UICalendarView.Decoration
```

## Parameters 

`image`  

An image to display as the decoration.

`color`  

A color for the decoration.

`size`  

A relative size for the decoration.

## Return Value

A calendar view decoration.

## Discussion

The image defaults to `circlebadge.fill` if you don’t specify it.

The color defaults to systemFill if you don’t specify it.

The size defaults to UICalendarView.DecorationSize.medium if nil.

