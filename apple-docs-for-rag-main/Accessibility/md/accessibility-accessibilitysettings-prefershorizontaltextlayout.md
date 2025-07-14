

- Accessibility
- AccessibilitySettings
-  prefersHorizontalTextLayout 

Type Property

# prefersHorizontalTextLayout

A Boolean value that indicates whether the system setting to prefer horizontal text for languages that support both vertical and horizontal text layout is on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var prefersHorizontalTextLayout: Bool { get }
```

## Discussion

The value of this property is true if the system setting for Prefer Horizontal Text is on; otherwise, false.

## See Also

### Customizing vertical text layout

Horizontal text

Lay out vertical text horizontally in your app when people turn on the Prefer Horizontal Text setting.

static var prefersHorizontalTextLayoutDidChangeNotification: Notification.Name

A notification that posts when the system setting to prefer horizontal text for languages that support both vertical and horizontal text layout changes.

