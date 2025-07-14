

- WebKit
- WKWebExtensionController
-  load(\_:) 

Instance Method

# load(\_:)

Loads the specified extension context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func load(_ extensionContext: WKWebExtensionContext) throws
```

## Discussion

Causes the context to start, loading any background content, and injecting any content into relevant tabs.

## See Also

### Related Documentation

func load(WKWebExtensionContext) throws

Loads the specified extension context.

