

- Swift
- Regex
- Regex.Match
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the capture with the specified name, if a capture with that name exists.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
subscript(name: String) -> AnyRegexOutput.Element? { get }
```

Available when `Output` is `AnyRegexOutput`.

## Parameters 

`name`  

The name of the capture to access.

## Return Value

An element providing information about the capture, if there is a capture named `name`; otherwise, `nil`.

