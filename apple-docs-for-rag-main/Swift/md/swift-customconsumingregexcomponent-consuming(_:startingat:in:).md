

- Swift
- CustomConsumingRegexComponent
-  consuming(\_:startingAt:in:) 

Instance Method

# consuming(\_:startingAt:in:)

Process the input string within the specified bounds, beginning at the given index, and return the end position (upper bound) of the match and the produced output.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func consuming(
    _ input: String,
    startingAt index: String.Index,
    in bounds: Range
) throws -> (upperBound: String.Index, output: Self.RegexOutput)?
```

**Required**

## Parameters 

`input`  

The string in which the match is performed.

`index`  

An index of `input` at which to begin matching.

`bounds`  

The bounds in `input` in which the match is performed.

## Return Value

The upper bound where the match terminates and a matched instance, or `nil` if there isn’t a match.

