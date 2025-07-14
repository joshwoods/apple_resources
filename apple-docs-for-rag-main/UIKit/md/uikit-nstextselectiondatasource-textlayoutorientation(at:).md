

- UIKit
- NSTextSelectionDataSource
-  textLayoutOrientation(at:) 

Instance Method

# textLayoutOrientation(at:)

Returns the layout orientation at the location you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func textLayoutOrientation(at location: any NSTextLocation) -> NSTextSelectionNavigation.LayoutOrientation
```

## Parameters 

`location`  

The location where you want to examine the text’s layout orientation.

## Return Value

Returns an NSTextSelectionNavigation.LayoutOrientation that describes the orientation of the layout.

## See Also

### Changing the characteristics of the selection

func baseWritingDirection(at: any NSTextLocation) -> NSTextSelectionNavigation.WritingDirection

Returns the base writing direction at the location you specify.

**Required**

enum WritingDirection

Values that describe the writing direction inside a text selection.

enum LayoutOrientation

Values that describe the possible layout orientations.

