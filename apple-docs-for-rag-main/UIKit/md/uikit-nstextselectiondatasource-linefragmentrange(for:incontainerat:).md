

- UIKit
- NSTextSelectionDataSource
-  lineFragmentRange(for:inContainerAt:) 

Instance Method

# lineFragmentRange(for:inContainerAt:)

Returns the range of the line fragment that contains the point you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func lineFragmentRange(
    for point: CGPoint,
    inContainerAt location: any NSTextLocation
) -> NSTextRange?
```

**Required**

## Parameters 

`point`  

The starting point that contains the line fragment, in the coordinate system of `location`.

`location`  

The location of the line fragment.

## Return Value

An `NSTextRange` that describes the location of the line fragment, or nil if the range isn’t found.

## See Also

### Finding specific content in the selection

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location using the location and offset you specify.

**Required**

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the offset between the two locations you specify.

**Required**

func textRange(for: NSTextSelection.Granularity, enclosing: any NSTextLocation) -> NSTextRange?

Returns a text range that corresponds to selection granularity of the enclosing location.

**Required**

