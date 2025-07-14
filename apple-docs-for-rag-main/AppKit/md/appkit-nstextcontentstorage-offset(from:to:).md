

- AppKit
- NSTextContentStorage
-  offset(from:to:) 

Instance Method

# offset(from:to:)

Returns the number of characters between the specified locations.

macOS 12.0+

``` source
func offset(
    from: any NSTextLocation,
    to: any NSTextLocation
) -> Int
```

## Parameters 

`from`  

The starting location in the text storage. For example, you might specify the beginning of the document as the starting location.

`to`  

The end location in the text storage.

## Return Value

The number of characters between the start and end locations. If the to location comes before the from location, the returned value is negative.

## Discussion

You can get NSTextLocation objects for the start and end of the text storage from the documentRange property of the NSTextElementProvider protocol, which NSTextContentStorage implements. If you provide an NSTextLocation object doesn’t match the type of the ones in the documentRange property, this method throws an exception.

## See Also

### Finding ranges, locations, and offsets

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new text location object based on an existing location and offset you provide.

func adjustedRange(from: NSTextRange, forEditingTextSelection: Bool) -> NSTextRange?

Returns the text range, if any, in the backing store that required manual adjustment after editing.

