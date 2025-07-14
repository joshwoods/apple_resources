

- AppKit
- NSTextSelectionDataSource
-  location(\_:offsetBy:) 

Instance Method

# location(\_:offsetBy:)

Returns a new location using the location and offset you specify.

macOS 12.0+

``` source
func location(
    _ location: any NSTextLocation,
    offsetBy offset: Int
) -> (any NSTextLocation)?
```

**Required**

## Parameters 

`location`  

The starting location in the selection.

`offset`  

An offset that describes the extent of the new location.

## Return Value

A new `NSTextLocation, or nil` when the inputs don’t produce any legal location, such as when the input is an out of bounds index.

## Discussion

The offset value can be positive or negative indicating the logical direction.

## See Also

### Finding specific content in the selection

func lineFragmentRange(for: CGPoint, inContainerAt: any NSTextLocation) -> NSTextRange?

Returns the range of the line fragment that contains the point you specify.

**Required**

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the offset between the two locations you specify.

**Required**

func textRange(for: NSTextSelection.Granularity, enclosing: any NSTextLocation) -> NSTextRange?

Returns a text range that corresponds to selection granularity of the enclosing location.

**Required**

