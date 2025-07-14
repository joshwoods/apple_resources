

- UIKit
- UIWritingToolsCoordinator
-  resultOptions 

Instance Property

# resultOptions

The type of content the system generates for your custom text view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
var resultOptions: UIWritingToolsResultOptions { get }
```

## Discussion

This property contains the set of options that Writing Tools outputs for your view. Writing Tools takes the value in the preferredResultOptions property into consideration when determining this value.

## See Also

### Configuring the experience

var preferredBehavior: UIWritingToolsBehavior

The level of Writing Tools support you want the system to provide for your view.

var behavior: UIWritingToolsBehavior

The actual level of Writing Tools support the system provides for your view.

var preferredResultOptions: UIWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

