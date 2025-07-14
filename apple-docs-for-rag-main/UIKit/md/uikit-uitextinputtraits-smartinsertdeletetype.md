

- UIKit
- UITextInputTraits
-  smartInsertDeleteType 

Instance Property

# smartInsertDeleteType

The configuration state for the smart insertion and deletion of space characters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional var smartInsertDeleteType: UITextSmartInsertDeleteType { get set }
```

## Discussion

Use this property to configure whether UIKit may insert an extra space after a paste operation or delete one or two spaces after a cut or delete operation. The default value of this property is UITextSmartInsertDeleteType.default, which selectively enables the behavior based on the keyboard type.

## See Also

### Configuring the autoformatting behaviors

var smartQuotesType: UITextSmartQuotesType

The configuration state for smart quotes.

enum UITextSmartQuotesType

Constants that indicate whether to enable or disable smart quotes.

var smartDashesType: UITextSmartDashesType

The configuration state for smart dashes.

enum UITextSmartDashesType

Constants that specify the automatic conversion behavior between hyphens and en or em dashes.

enum UITextSmartInsertDeleteType

Constants that specify whether to automatically insert extra spaces after a paste operation or to delete them after a cut or delete operation.

