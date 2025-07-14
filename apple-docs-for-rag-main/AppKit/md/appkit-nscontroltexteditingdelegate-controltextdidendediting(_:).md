

- AppKit
- NSControlTextEditingDelegate
-  controlTextDidEndEditing(\_:) 

Instance Method

# controlTextDidEndEditing(\_:)

Tells the delegate that the control finished editing its text content and committed the changes.

macOS 10.10+

``` source
@MainActor
optional func controlTextDidEndEditing(_ obj: Notification)
```

## Parameters 

`obj`  

A notification object that contains details about the editing configuration.

## Discussion

Use the key `“NSFieldEditor”` to obtain the field editor from the notification object’s `userInfo` dictionary.

Note

If you call abortEditing() to discard pending edits, the control doesn’t call controlTextDidEndEditing(_:).

## See Also

### Instance Methods

func controlTextDidBeginEditing(Notification)

Tells the delegate that the control started editing its text content.

func controlTextDidChange(Notification)

Tells the delegate that the control made changes to its text content.

