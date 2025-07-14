

- WebKit
- WKWebView
-  init(coder:) 

Initializer

# init(coder:)

Returns an object initialized from data in the specified coder object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder object that contains the object’s data.

## See Also

### Creating a web view

init(frame: CGRect, configuration: WKWebViewConfiguration)

Creates a web view and initializes it with the specified frame and configuration data.

var configuration: WKWebViewConfiguration

The object that contains the configuration details for the web view.

