

- AppKit
- NSTextContentStorage
-  location(\_:offsetBy:) 

Instance Method

# location(\_:offsetBy:)

Returns a new text location object based on an existing location and offset you provide.

macOS 12.0+

``` source
func location(
    _ location: any NSTextLocation,
    offsetBy offset: Int
) -> (any NSTextLocation)?
```

## Parameters 

`location`  

The starting location. For example, you might specify the beginning or end of the document as the starting location.

`offset`  

The number of characters from the starting location. Specify a positive integer to create a location object that comes after the starting location. Specify a negative number to create a location object that comes before the starting location.

## Return Value

An NSTextLocation object that corresponds to the new location, or `nil` if the new location exceeds the bounds of the text.

## Discussion

You can get NSTextLocation objects for the start and end of the text storage from the documentRange property of the NSTextElementProvider protocol, which NSTextContentStorage implements. If you provide an NSTextLocation object doesn’t match the type of the ones in the documentRange property, this method throws an exception.

## See Also

### Finding ranges, locations, and offsets

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the number of characters between the specified locations.

func adjustedRange(from: NSTextRange, forEditingTextSelection: Bool) -> NSTextRange?

Returns the text range, if any, in the backing store that required manual adjustment after editing.

