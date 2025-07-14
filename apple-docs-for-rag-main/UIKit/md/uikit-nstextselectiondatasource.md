

- UIKit
-  NSTextSelectionDataSource 

Protocol

# NSTextSelectionDataSource

A set of methods that objects implement to provide data for, and manage text selections.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
protocol NSTextSelectionDataSource : NSObjectProtocol
```

## Topics

### Range of the selection

var documentRange: NSTextRange

Returns the starting and ending locations for the document.

**Required**

### Enumerating components of the selection

func enumerateCaretOffsetsInLineFragment(at: any NSTextLocation, using: (CGFloat, any NSTextLocation, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the insertion point caret offsets from left to right in visual order.

**Required**

func enumerateContainerBoundaries(from: any NSTextLocation, reverse: Bool, using: (any NSTextLocation, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the container boundaries starting from the location you specify.

func enumerateSubstrings(from: any NSTextLocation, options: NSString.EnumerationOptions, using: (String?, NSTextRange, NSTextRange?, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the textual segment boundaries starting at the location you specify.

**Required**

### Finding specific content in the selection

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location using the location and offset you specify.

**Required**

func lineFragmentRange(for: CGPoint, inContainerAt: any NSTextLocation) -> NSTextRange?

Returns the range of the line fragment that contains the point you specify.

**Required**

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the offset between the two locations you specify.

**Required**

func textRange(for: NSTextSelection.Granularity, enclosing: any NSTextLocation) -> NSTextRange?

Returns a text range that corresponds to selection granularity of the enclosing location.

**Required**

### Changing the characteristics of the selection

func baseWritingDirection(at: any NSTextLocation) -> NSTextSelectionNavigation.WritingDirection

Returns the base writing direction at the location you specify.

**Required**

enum WritingDirection

Values that describe the writing direction inside a text selection.

func textLayoutOrientation(at: any NSTextLocation) -> NSTextSelectionNavigation.LayoutOrientation

Returns the layout orientation at the location you specify.

enum LayoutOrientation

Values that describe the possible layout orientations.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextLayoutManager

## See Also

### Accessing the data source

var textSelectionDataSource: (any NSTextSelectionDataSource)?

The data source associated with this selection navigation.

