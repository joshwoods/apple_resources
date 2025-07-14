

- Core Text
-  CTTypesetterSuggestClusterBreak(\_:\_:\_:) 

Function

# CTTypesetterSuggestClusterBreak(\_:\_:\_:)

Suggests a cluster line breakpoint based on the width provided.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTypesetterSuggestClusterBreak(
    _ typesetter: CTTypesetter,
    _ startIndex: CFIndex,
    _ width: Double
) -> CFIndex
```

## Parameters 

`typesetter`  

The typesetter that creates the line. This parameter is required and cannot be set to `NULL`.

`startIndex`  

The starting point for the typographic cluster-break calculations. The break calculations include the character starting at `startIndex`.

`width`  

The requested typographic cluster-break width.

## Return Value

A count of the characters from `startIndex` that would cause the cluster break. The value returned can be used to construct a character range for CTTypesetterCreateLine(_:_:).

## Discussion

This cluster break is similar to a character break, except that it does not break apart linguistic clusters. No other contextual analysis is done. This can be used by the caller to implement a different line-breaking scheme, such as hyphenation. A typographic cluster break can also be triggered by a hard-break character in the stream. This function is equivalent to CTTypesetterSuggestClusterBreakWithOffset(_:_:_:_:) with an offset of 0.0.

## See Also

### Breaking Lines

func CTTypesetterSuggestLineBreak(CTTypesetter, CFIndex, Double) -> CFIndex

Suggests a contextual line breakpoint based on the width provided.

func CTTypesetterSuggestLineBreakWithOffset(CTTypesetter, CFIndex, Double, Double) -> CFIndex

Suggests a contextual line breakpoint based on the width provided and the specified offset.

func CTTypesetterSuggestClusterBreakWithOffset(CTTypesetter, CFIndex, Double, Double) -> CFIndex

Suggests a cluster line breakpoint based on the specified width and line offset.

