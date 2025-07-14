

- Swift
- Regex
-  init(\_:) 

Initializer

# init(\_:)

Creates a regular expression with a dynamic capture list from the given regular expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ regex: Regex)
```

Available when `Output` is `AnyRegexOutput`.

## Parameters 

`regex`  

A regular expression to convert to use a dynamic capture list.

## Discussion

You can use this initializer to convert a `Regex` with strongly-typed captures into a `Regex` with `AnyRegexOutput` as its output type.

