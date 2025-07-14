

- UIKit
- UIScrollView
-  keyboardDismissMode 

Instance Property

# keyboardDismissMode

The manner in which the system dismisses the keyboard when a drag begins in the scroll view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var keyboardDismissMode: UIScrollView.KeyboardDismissMode { get set }
```

## Discussion

The default value is UIScrollView.KeyboardDismissMode.none. See UIScrollView.KeyboardDismissMode for possible values.

## See Also

### Dismissing the keyboard

enum KeyboardDismissMode

Constants that determine how the system dismisses the keyboard when a drag begins in the scroll view.

