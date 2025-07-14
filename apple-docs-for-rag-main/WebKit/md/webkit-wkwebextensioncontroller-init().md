

- WebKit
- WKWebExtensionController
-  init() 

Initializer

# init()

Returns a web extension controller initialized with the default configuration.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
init()
```

## Return Value

An initialized web extension controller, or nil if the object could not be initialized.

## Discussion

This is a designated initializer. You can use init(configuration:) to initialize an instance with a configuration.

## See Also

### Related Documentation

init(configuration: WKWebExtensionController.Configuration)

Returns a web extension controller initialized with the specified configuration.

