

- Swift
- AnyRegexOutput
-  init(\_:) 

Initializer

# init(\_:)

Creates a dynamic regular expression match output from an existing match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ match: Regex.Match)
```

## Discussion

You can use this initializer when you need an `AnyRegexOutput` instance instead of the output type of a strongly-typed `Regex.Match`.

