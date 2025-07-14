

- UIKit
- UITextSmartInsertDeleteType
-  UITextSmartInsertDeleteType.default 

Case

# UITextSmartInsertDeleteType.default

Use the default behavior for inserting and deleting space characters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
case `default`
```

## Discussion

This option selectively enables the automatic deletion of one or two neighboring spaces after a cut or delete, and the insertion of an extra space after a paste. For example, this option disables the behavior for email address and password keyboards.

## See Also

### Constants

case no

Disable the insertion or deletion of extra spaces.

case yes

Enable the insertion or deletion of extra spaces.

