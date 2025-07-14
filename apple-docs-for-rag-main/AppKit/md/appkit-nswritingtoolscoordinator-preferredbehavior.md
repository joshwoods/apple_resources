

- AppKit
- NSWritingToolsCoordinator
-  preferredBehavior 

Instance Property

# preferredBehavior

The level of Writing Tools support you want the system to provide for your view.

macOS 15.2+

``` source
@MainActor
var preferredBehavior: NSWritingToolsBehavior { get set }
```

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Discussion

Use this property to request an inline or panel-based experience, or to disable Writing Tools for your view altogether. The default value of this property is NSWritingToolsBehavior.default.

## See Also

### Configuring the experience

var behavior: NSWritingToolsBehavior

The actual level of Writing Tools support the system provides for your view.

var preferredResultOptions: NSWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

var resultOptions: NSWritingToolsResultOptions

The type of content the system generates for your custom text view.

