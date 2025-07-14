

- WebKit
- WKWebView
-  uiDelegate 

Instance Property

# uiDelegate

The object you use to integrate custom user interface elements, such as contextual menus or panels, into web view interactions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
weak var uiDelegate: (any WKUIDelegate)? { get set }
```

## See Also

### Displaying native user interface elements

protocol WKUIDelegate

The methods for presenting native user interface elements on behalf of a webpage.

