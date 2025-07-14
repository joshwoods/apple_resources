

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  init(string:) 

Initializer

# init(string:)

Returns a pattern object for the specified pattern string.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
init(string: String) throws
```

## Parameters 

`string`  

On output, a pointer to an error object that describes why the method failed, or `nil` if no error occurred. If you are not interested in the error information, pass `nil` for this parameter.

## Return Value

A pattern object, or `nil` if the pattern string is invalid and an error will be set.

