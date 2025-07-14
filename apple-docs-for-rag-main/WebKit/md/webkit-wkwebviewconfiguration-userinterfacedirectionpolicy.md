

- WebKit
- WKWebViewConfiguration
-  userInterfaceDirectionPolicy 

Instance Property

# userInterfaceDirectionPolicy

The directionality of user interface elements.

macOS 10.12+

``` source
@MainActor
var userInterfaceDirectionPolicy: WKUserInterfaceDirectionPolicy { get set }
```

## Discussion

The default value is WKUserInterfaceDirectionPolicy.content. For other possible values, see WKUserInterfaceDirectionPolicy.

## See Also

### Selecting user interface directionality

enum WKUserInterfaceDirectionPolicy

The policy that determines the directionality of user interface elements in a web view.

