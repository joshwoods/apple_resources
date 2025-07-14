

- AVFoundation
- AVCaption
-  backgroundColor(at:) 

Instance Method

# backgroundColor(at:)

Returns the background color at the index position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
@nonobjc
func backgroundColor(at index: String.Index) -> (CGColor?, Range)
```

## Parameters 

`index`  

A character position in the caption text.

## Return Value

A tuple that contains the background color and range to which it applies.

## See Also

### Accessing Colors

func textColor(at: String.Index) -> (CGColor?, Range&lt;String.Index>)

Returns the text color at the index position.

