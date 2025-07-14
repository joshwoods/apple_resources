

- AppKit
- NSWritingToolsCoordinator
-  resultOptions 

Instance Property

# resultOptions

The type of content the system generates for your custom text view.

macOS 15.2+

``` source
@MainActor
var resultOptions: NSWritingToolsResultOptions { get }
```

## Discussion

This property contains the set of options that Writing Tools outputs for your view. Writing Tools takes the value in the preferredResultOptions property into consideration when determining this value.

## See Also

### Configuring the experience

var preferredBehavior: NSWritingToolsBehavior

The level of Writing Tools support you want the system to provide for your view.

var behavior: NSWritingToolsBehavior

The actual level of Writing Tools support the system provides for your view.

var preferredResultOptions: NSWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

