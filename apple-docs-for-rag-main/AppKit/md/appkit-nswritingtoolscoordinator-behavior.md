

- AppKit
- NSWritingToolsCoordinator
-  behavior 

Instance Property

# behavior

The actual level of Writing Tools support the system provides for your view.

macOS 15.2+

``` source
@MainActor
var behavior: NSWritingToolsBehavior { get }
```

## Discussion

The system chooses this value based on the device capabilities, and takes the value in the preferredBehavior property into consideration when making the choice. The value in this property is never the default option, and is instead one of the specific options such as NSWritingToolsBehavior.none, NSWritingToolsBehavior.limited, or NSWritingToolsBehavior.complete.

## See Also

### Configuring the experience

var preferredBehavior: NSWritingToolsBehavior

The level of Writing Tools support you want the system to provide for your view.

var preferredResultOptions: NSWritingToolsResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

var resultOptions: NSWritingToolsResultOptions

The type of content the system generates for your custom text view.

