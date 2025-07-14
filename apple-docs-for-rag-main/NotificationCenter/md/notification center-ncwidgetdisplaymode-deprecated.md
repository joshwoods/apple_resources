

- Notification Center
-  NCWidgetDisplayMode Deprecated

Enumeration

# NCWidgetDisplayMode

The modes that can be toggled between when the user activates the More button for a widget running in iOS.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 10.0–14.0Deprecated

``` source
enum NCWidgetDisplayMode
```

Deprecated

Use WidgetKit instead.

## Topics

### Constants

case compact

The current height of the widget is compact.

case expanded

The current height of the widget is expanded.

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

### Customizing the Display

func widgetMarginInsets(forProposedMarginInsets: UIEdgeInsets) -> UIEdgeInsets

Called to let a widget accept the default margin inset values or return custom values to use instead.

Deprecated

func widgetActiveDisplayModeDidChange(NCWidgetDisplayMode, withMaximumSize: CGSize)

Called when the active display mode changes.

Deprecated

