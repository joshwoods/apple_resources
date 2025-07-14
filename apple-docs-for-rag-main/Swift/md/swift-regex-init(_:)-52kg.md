

- Swift
- Regex
-  init(\_:) 

Initializer

# init(\_:)

Creates a regular expression from the given string, using a dynamic capture list.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ pattern: String) throws
```

Available when `Output` is `AnyRegexOutput`.

## Parameters 

`pattern`  

A string with regular expression syntax.

## Discussion

Use this initializer to create a `Regex` instance from a regular expression that you have stored in `pattern`.

```
let simpleDigits = try Regex("[0-9]+")
```

This initializer throws an error if `pattern` uses invalid regular expression syntax.

The output type of the new `Regex` is the dynamic AnyRegexOutput. If you know the capture structure of `pattern` ahead of time, use the `init(_:as:)` initializer instead.

