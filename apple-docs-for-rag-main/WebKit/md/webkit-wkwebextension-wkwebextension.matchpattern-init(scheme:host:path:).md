

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  init(scheme:host:path:) 

Initializer

# init(scheme:host:path:)

Returns a pattern object for the specified scheme, host, and path strings.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
init(
    scheme: String,
    host: String,
    path: String
) throws
```

## Parameters 

`scheme`  

On output, a pointer to an error object that describes why the method failed, or `nil` if no error occurred. If you are not interested in the error information, pass `nil` for this parameter.

## Return Value

A pattern object, or `nil` if any of the strings are invalid and an error will be set.

