

- AppKit
- NSComboBox
-  completes 

Instance Property

# completes

A Boolean value indicating whether the combo box tries to complete what the user types.

macOS

``` source
@MainActor
var completes: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box tries to complete what the user is typing. Every time the user types a new character, the combo box uses the completedString(_:) method of its cell to get the new value. If the string returned by that method is longer than the string typed by the user, the combo box replaces the existing string with the returned string and selects the additional characters. If the user is deleting characters or adds characters somewhere besides the end of the string, the combo box does not try to complete it.

When the value of this property is false, the combo box does not try to complete the string typed by the user.

