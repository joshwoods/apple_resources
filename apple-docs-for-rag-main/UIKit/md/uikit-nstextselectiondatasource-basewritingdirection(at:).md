

- UIKit
- NSTextSelectionDataSource
-  baseWritingDirection(at:) 

Instance Method

# baseWritingDirection(at:)

Returns the base writing direction at the location you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func baseWritingDirection(at location: any NSTextLocation) -> NSTextSelectionNavigation.WritingDirection
```

**Required**

## Parameters 

`location`  

The location where you want to examine the text’s writing direction.

## Return Value

The NSWritingDirection.

## See Also

### Changing the characteristics of the selection

enum WritingDirection

Values that describe the writing direction inside a text selection.

func textLayoutOrientation(at: any NSTextLocation) -> NSTextSelectionNavigation.LayoutOrientation

Returns the layout orientation at the location you specify.

enum LayoutOrientation

Values that describe the possible layout orientations.

