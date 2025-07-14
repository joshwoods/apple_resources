

- UIKit
- UIPickerView
-  showsSelectionIndicator Deprecated

Instance Property

# showsSelectionIndicator

A Boolean value that determines whether the selection indicator is displayed.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var showsSelectionIndicator: Bool { get set }
```

Deprecated

In iOS 7 and later, you can’t customize the picker view’s selection indicator. The selection indicator is always shown, so setting this property to false has no effect.

## Discussion

If the value of the property is true, the picker view shows a clear overlay across the current row. The default value of this property is false.

