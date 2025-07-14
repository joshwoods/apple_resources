

- UIKit
- UIWritingToolsCoordinator
-  preferredBehavior 

Instance Property

# preferredBehavior

The level of Writing Tools support you want the system to provide for your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
var preferredBehavior: UIWritingToolsBehavior { get set }
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

Use this property to request an inline or panel-based experience, or to disable Writing Tools for your view altogether. The default value of this property is UIWritingToolsBehavior.default.

## See Also

### Configuring the experience

var behavior: UIWritingToolsBehavior

The actual level of Writing Tools support the system provides for your view.

var preferredResultOptions: UIWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

var resultOptions: UIWritingToolsResultOptions

The type of content the system generates for your custom text view.

