

- WebKit
- WKWebExtension
-  hasOptionsPage 

Instance Property

# hasOptionsPage

A Boolean value indicating whether the extension has an options page.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasOptionsPage: Bool { get }
```

## Discussion

If this property is `YES`, the extension includes a dedicated options page where users can customize settings. The app should provide access to this page through a user interface element, which can be accessed via optionsPageURL on an extension context.

