

- Swift
- Regex
-  init(\_:as:) 

Initializer

# init(\_:as:)

Creates a regular expression with a strongly-typed capture list from the given regular expression.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init?(
    _ regex: Regex,
    as outputType: Output.Type = Output.self
)
```

## Parameters 

`regex`  

A regular expression to convert to use a strongly-typed capture list.

`outputType`  

The capture structure to use.

## Discussion

You can use this initializer to convert a regular expression with a dynamic capture list to one with a strongly-typed capture list. If the type you provide as `outputType` doesn’t match the capture structure of `regex`, the initializer returns `nil`.

```
let dynamicRegex = try Regex("(.+?): (.+)")
if let stronglyTypedRegex = Regex(dynamicRegex, as: (Substring, Substring, Substring).self) {
    print("Converted properly")
}
// Prints "Converted properly"
```

