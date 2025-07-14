

- AppKit
- NSTextSelectionDataSource
-  offset(from:to:) 

Instance Method

# offset(from:to:)

Returns the offset between the two locations you specify.

macOS 12.0+

``` source
func offset(
    from: any NSTextLocation,
    to: any NSTextLocation
) -> Int
```

**Required**

## Parameters 

`from`  

The starting location.

`to`  

The ending location.

## See Also

### Finding specific content in the selection

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location using the location and offset you specify.

**Required**

func lineFragmentRange(for: CGPoint, inContainerAt: any NSTextLocation) -> NSTextRange?

Returns the range of the line fragment that contains the point you specify.

**Required**

func textRange(for: NSTextSelection.Granularity, enclosing: any NSTextLocation) -> NSTextRange?

Returns a text range that corresponds to selection granularity of the enclosing location.

**Required**

