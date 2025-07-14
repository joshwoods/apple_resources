

- Swift
- Regex
-  anchorsMatchLineEndings(\_:) 

Instance Method

# anchorsMatchLineEndings(\_:)

Returns a regular expression where the start and end of input anchors (`^` and `$`) also match against the start and end of a line.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func anchorsMatchLineEndings(_ matchLineEndings: Bool = true) -> Regex.RegexOutput>
```

## Parameters 

`matchLineEndings`  

A Boolean value indicating whether `^` and `$` should match the start and end of lines, respectively.

## Return Value

The modified regular expression.

## Discussion

This method corresponds to applying the `m` option in regex syntax. For this behavior in the `RegexBuilder` syntax, see `Anchor.startOfLine`, `Anchor.endOfLine`, `Anchor.startOfSubject`, and `Anchor.endOfSubject`.

