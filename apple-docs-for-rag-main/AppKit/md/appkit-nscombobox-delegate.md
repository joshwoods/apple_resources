

- AppKit
- NSComboBox
-  delegate 

Instance Property

# delegate

Sets the receiver’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSComboBoxDelegate)? { get set }
```

## Parameters 

`anObject`  

The delegate for the receiver. The delegate must conform to the NSComboBoxDelegate protocol.

