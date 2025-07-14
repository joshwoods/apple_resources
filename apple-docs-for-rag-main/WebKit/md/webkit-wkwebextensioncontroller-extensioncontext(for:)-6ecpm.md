

- WebKit
- WKWebExtensionController
-  extensionContext(for:) 

Instance Method

# extensionContext(for:)

Returns a loaded extension context for the specified extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func extensionContext(for extension: WKWebExtension) -> WKWebExtensionContext?
```

## Parameters 

`extension`  

An extension to lookup.

## Return Value

An extension context or `nil` if no match was found.

## See Also

### Related Documentation

var extensions: Set&lt;WKWebExtension>

A set of all the currently loaded extensions.

