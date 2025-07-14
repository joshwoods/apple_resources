

- Swift
- Regex
-  wordBoundaryKind(\_:) 

Instance Method

# wordBoundaryKind(\_:)

Returns a regular expression that uses the specified word boundary algorithm.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func wordBoundaryKind(_ wordBoundaryKind: RegexWordBoundaryKind) -> Regex.RegexOutput>
```

## Parameters 

`wordBoundaryKind`  

The algorithm to use for determining word boundaries.

## Return Value

The modified regular expression.

