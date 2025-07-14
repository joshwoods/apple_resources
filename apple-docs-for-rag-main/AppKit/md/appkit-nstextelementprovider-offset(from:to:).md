

- AppKit
- NSTextElementProvider
-  offset(from:to:) 

Instance Method

# offset(from:to:)

Returns the offset between the two specified locations.

macOS 12.0+

``` source
optional func offset(
    from: any NSTextLocation,
    to: any NSTextLocation
) -> Int
```

## Parameters 

`from`  

A starting location.

`to`  

An ending location.

## Return Value

An `Integer` that represents the offset between the starting and ending locations.

## Discussion

The return value could be positive or negative. This method can return NSNotFound when the method can’t represent an offset as an integer value. This can occur, for example, if the locations aren’t in the same document).

## See Also

### Adjusting the range of the text element

func adjustedRange(from: NSTextRange, forEditingTextSelection: Bool) -> NSTextRange?

A method you implement if the location backing store requires manual adjustment after editing.

