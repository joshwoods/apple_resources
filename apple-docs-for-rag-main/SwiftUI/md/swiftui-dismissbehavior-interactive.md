

- SwiftUI
- DismissBehavior
-  interactive 

Type Property

# interactive

The interactive dismiss behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let interactive: DismissBehavior
```

## Discussion

Use this behavior when you want to dismiss a window in a manner that is similar to the standard system affordances for window dismissal - for example, when a user clicks the close button.

This is the default behavior on macOS and iOS.

On macOS, dismissing a window using this behavior will not dismiss a window which is currently showing a modal presentation, such as a sheet or alert. Additionally, a document window that is dismissed with this behavior will show the save dialog if there are unsaved changes to the document.

On iOS, dismissing a window using this behavior will dismiss it regardless of any modal presentations being shown.

## See Also

### Getting behaviors

static let destructive: DismissBehavior

The destructive dismiss behavior.

