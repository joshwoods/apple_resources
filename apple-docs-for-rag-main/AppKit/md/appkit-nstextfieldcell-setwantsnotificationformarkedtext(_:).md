

- AppKit
- NSTextFieldCell
-  setWantsNotificationForMarkedText(\_:) 

Instance Method

# setWantsNotificationForMarkedText(\_:)

Directs the cell’s associated field editor to post text change notifications.

macOS 10.5+

``` source
@MainActor
func setWantsNotificationForMarkedText(_ flag: Bool)
```

## Parameters 

`flag`  

If true, the field editor posts text change notifications (NSTextDidChangeNotification) while editing marked text; if false, notifications are delayed until the marked text confirmation.

## See Also

### Managing the Field Editor

func setUpFieldEditorAttributes(NSText) -> NSText

Allows the cell to set up the field editor’s attributes before editing begins.

