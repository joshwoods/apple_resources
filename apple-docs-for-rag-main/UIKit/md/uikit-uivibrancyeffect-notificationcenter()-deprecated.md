

- UIKit
- UIVibrancyEffect
-  notificationCenter() Deprecated

Type Method

# notificationCenter()

Creates a vibrancy effect for use in Notification Center.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0Deprecated

``` source
@MainActor
class func notificationCenter() -> UIVibrancyEffect
```

Deprecated

Use widgetPrimary() instead.

## Return Value

The vibrancy effect that’s appropriate for use in Today widgets in Notification Center. To learn more about Today widgets, see Today.

## See Also

### Deprecated

class func widgetPrimary() -> UIVibrancyEffect

Creates a vibrancy effect suitable for use with certain supporting text and template images within a widget.

Deprecated

class func widgetSecondary() -> UIVibrancyEffect

Creates a vibrancy effect suitable for indicating the secondary importance or relevance of supporting text and template images within a widget.

Deprecated

class func widgetEffect(forVibrancyStyle: UIVibrancyEffectStyle) -> UIVibrancyEffect

Creates a vibrancy effect for the specified style.

Deprecated

