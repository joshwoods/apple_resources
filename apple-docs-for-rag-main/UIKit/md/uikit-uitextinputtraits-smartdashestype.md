

- UIKit
- UITextInputTraits
-  smartDashesType 

Instance Property

# smartDashesType

The configuration state for smart dashes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional var smartDashesType: UITextSmartDashesType { get set }
```

## Discussion

Use this property to configure whether UIKit converts two hyphens into an en-dash and three hyphens into an em-dash automatically. The default value of this property is UITextSmartDashesType.default, which selectively enables smart dashes based on the keyboard type.

## See Also

### Configuring the autoformatting behaviors

var smartQuotesType: UITextSmartQuotesType

The configuration state for smart quotes.

enum UITextSmartQuotesType

Constants that indicate whether to enable or disable smart quotes.

enum UITextSmartDashesType

Constants that specify the automatic conversion behavior between hyphens and en or em dashes.

var smartInsertDeleteType: UITextSmartInsertDeleteType

The configuration state for the smart insertion and deletion of space characters.

enum UITextSmartInsertDeleteType

Constants that specify whether to automatically insert extra spaces after a paste operation or to delete them after a cut or delete operation.

