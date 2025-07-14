

- AppKit
- NSTextSelectionDataSource
-  textRange(for:enclosing:) 

Instance Method

# textRange(for:enclosing:)

Returns a text range that corresponds to selection granularity of the enclosing location.

macOS 12.0+

``` source
func textRange(
    for selectionGranularity: NSTextSelection.Granularity,
    enclosing location: any NSTextLocation
) -> NSTextRange?
```

**Required**

## Parameters 

`selectionGranularity`  

One of the possible NSTextSelection.Granularity options.

`location`  

A location that encloses the text range of interest.

## Return Value

Returns the text range of the section, or `nil` when `documentRange.isEmpty` `true`.

## See Also

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

