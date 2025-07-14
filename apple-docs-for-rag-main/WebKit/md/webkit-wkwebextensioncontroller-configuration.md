

- WebKit
- WKWebExtensionController
-  configuration 

Instance Property

# configuration

A copy of the configuration with which the web extension controller was initialized.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@NSCopying @MainActor
var configuration: WKWebExtensionController.Configuration { get }
```

## Discussion

Mutating the configuration has no effect on the web extension controller.

