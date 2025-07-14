

- Accessibility
- AccessibilitySettings
-  animatedImagesEnabled 

Type Property

# animatedImagesEnabled

A Boolean value that indicates whether the system setting for playing animated images is on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var animatedImagesEnabled: Bool { get }
```

## Discussion

The value of this property is true if the system setting for Animated Images is on; otherwise, false.

## See Also

### Pausing animated images

Animated images

Pause animations in animated images in your app when people turn off the Animated Images setting.

static var animatedImagesEnabledDidChangeNotification: Notification.Name

A notification that posts when the system setting for playing animated images changes.

