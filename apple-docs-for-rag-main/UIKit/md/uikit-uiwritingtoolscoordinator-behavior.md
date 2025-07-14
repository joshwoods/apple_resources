

- UIKit
- UIWritingToolsCoordinator
-  behavior 

Instance Property

# behavior

The actual level of Writing Tools support the system provides for your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
var behavior: UIWritingToolsBehavior { get }
```

## Discussion

The system chooses this value based on the device capabilities, and takes the value in the preferredBehavior property into consideration when making the choice. The value in this property is never the default option, and is instead one of the specific options such as UIWritingToolsBehavior.none, UIWritingToolsBehavior.limited, or UIWritingToolsBehavior.complete.

## See Also

### Configuring the experience

var preferredBehavior: UIWritingToolsBehavior

The level of Writing Tools support you want the system to provide for your view.

var preferredResultOptions: UIWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

var resultOptions: UIWritingToolsResultOptions

The type of content the system generates for your custom text view.

