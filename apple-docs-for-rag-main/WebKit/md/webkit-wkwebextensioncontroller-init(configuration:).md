

- WebKit
- WKWebExtensionController
-  init(configuration:) 

Initializer

# init(configuration:)

Returns a web extension controller initialized with the specified configuration.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
init(configuration: WKWebExtensionController.Configuration)
```

## Parameters 

`configuration`  

The configuration for the new web extension controller.

## Return Value

An initialized web extension controller, or nil if the object could not be initialized.

## Discussion

This is a designated initializer. You can use init() to initialize an instance with the default configuration. The initializer copies the specified configuration, so mutating the configuration after invoking the initializer has no effect on the web extension controller.

## See Also

### Related Documentation

init()

Returns a web extension controller initialized with the default configuration.

