

- SwiftUI
- EnvironmentValues
-  accessibilityLargeContentViewerEnabled 

Instance Property

# accessibilityLargeContentViewerEnabled

Whether the Large Content Viewer is enabled.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var accessibilityLargeContentViewerEnabled: Bool { get }
```

## Discussion

The system can automatically provide a large content view with accessibilityShowsLargeContentViewer() or you can provide your own with accessibilityShowsLargeContentViewer(_:).

While it is not necessary to check this value before adding a large content view, it may be helpful if you need to adjust the behavior of a gesture. For example, a button with a long press handler might increase its long press duration so the user can read the text in the large content viewer first.

## See Also

### Enlarging content

func accessibilityShowsLargeContentViewer() -> some View

Adds a default large content view to be shown by the large content viewer.

func accessibilityShowsLargeContentViewer&lt;V>(() -> V) -> some View

Adds a custom large content view to be shown by the large content viewer.

