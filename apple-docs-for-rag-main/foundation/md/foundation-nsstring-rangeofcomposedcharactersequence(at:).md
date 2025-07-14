

- Foundation
- NSString
-  rangeOfComposedCharacterSequence(at:) 

Instance Method

# rangeOfComposedCharacterSequence(at:)

Returns the range in the receiver of the composed character sequence located at a given index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfComposedCharacterSequence(at index: Int) -> NSRange
```

## Parameters 

`index`  

The index of a character in the receiver. The value must not exceed the bounds of the receiver.

## Return Value

The range in the receiver of the composed character sequence located at `anIndex`.

## Discussion

The composed character sequence includes the first decomposed base letter found at or before `anIndex`, and its length includes the decomposed base letter and all combining characters that follow.

## See Also

### Determining Composed Character Sequences

func rangeOfComposedCharacterSequences(for: NSRange) -> NSRange

Returns the range in the string of the composed character sequences for a given range.

