

- AppKit
- NSControlTextEditingDelegate
-  controlTextDidChange(\_:) 

Instance Method

# controlTextDidChange(\_:)

Tells the delegate that the control made changes to its text content.

macOS 10.10+

``` source
@MainActor
optional func controlTextDidChange(_ obj: Notification)
```

## Parameters 

`obj`  

A notification object that contains details about the editing configuration.

## Discussion

Use the key `“NSFieldEditor”` to obtain the field editor from the notification object’s `userInfo` dictionary.

## See Also

### Instance Methods

func controlTextDidBeginEditing(Notification)

Tells the delegate that the control started editing its text content.

func controlTextDidEndEditing(Notification)

Tells the delegate that the control finished editing its text content and committed the changes.

