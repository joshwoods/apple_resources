

- UIKit
-  UITextSmartDashesType 

Enumeration

# UITextSmartDashesType

Constants that specify the automatic conversion behavior between hyphens and en or em dashes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum UITextSmartDashesType
```

## Topics

### Constants

case `default`

Use the default smart dash behavior.

case no

Disable smart dashes.

case yes

Enable smart dashes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the autoformatting behaviors

var smartQuotesType: UITextSmartQuotesType

The configuration state for smart quotes.

enum UITextSmartQuotesType

Constants that indicate whether to enable or disable smart quotes.

var smartDashesType: UITextSmartDashesType

The configuration state for smart dashes.

var smartInsertDeleteType: UITextSmartInsertDeleteType

The configuration state for the smart insertion and deletion of space characters.

enum UITextSmartInsertDeleteType

Constants that specify whether to automatically insert extra spaces after a paste operation or to delete them after a cut or delete operation.

