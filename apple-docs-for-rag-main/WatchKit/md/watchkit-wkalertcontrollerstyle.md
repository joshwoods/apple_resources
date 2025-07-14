

- WatchKit
-  WKAlertControllerStyle 

Enumeration

# WKAlertControllerStyle

Constants indicating the styles for standard system alerts.

watchOS 2.0+

``` source
enum WKAlertControllerStyle
```

## Topics

### Constants

case alert

An alert sheet with stacked buttons. The alert sheet includes a default Cancel button at the bottom of the sheet. You can add other buttons, which are placed above the Cancel button.

case sideBySideButtonsAlert

An alert sheet with side-by-side buttons.

case actionSheet

An action sheet style. Action sheets are modal sheets that can be dismissed using the Cancel button in the top-left corner of the sheet. You can also add one or two custom buttons to perform related tasks.

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

### Presenting interface controllers modally

func presentController(withName: String, context: Any?)

Presents a single interface controller modally.

func presentController(withNames: [String], contexts: [Any]?)

Presents a page-based interface modally.

func presentController(withNamesAndContexts: [(name: String, context: AnyObject)])

Presents a page-based interface modally.

func presentAlert(withTitle: String?, message: String?, preferredStyle: WKAlertControllerStyle, actions: [WKAlertAction])

Presents an alert or action sheet over the current interface controller.

func dismiss()

Dismisses the current interface controller from the screen.

