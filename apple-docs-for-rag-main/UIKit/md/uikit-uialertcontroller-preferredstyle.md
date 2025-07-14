

- UIKit
- UIAlertController
-  preferredStyle 

Instance Property

# preferredStyle

The style of the alert controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredStyle: UIAlertController.Style { get }
```

## Discussion

The value of this property is set to the value you specified in the init(title:message:preferredStyle:) method. This value determines how the alert is displayed onscreen.

## See Also

### Configuring the alert

var title: String?

The title of the alert.

var message: String?

Descriptive text that provides more details about the reason for the alert.

