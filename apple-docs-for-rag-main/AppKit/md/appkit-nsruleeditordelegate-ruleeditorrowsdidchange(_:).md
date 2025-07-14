

- AppKit
- NSRuleEditorDelegate
-  ruleEditorRowsDidChange(\_:) 

Instance Method

# ruleEditorRowsDidChange(\_:)

Notifies the receiver that a rule editor’s rows changed.

macOS 10.10+

``` source
@MainActor
optional func ruleEditorRowsDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

A notification namedrowsDidChangeNotification.

## Discussion

If the delegate implements this method, NSRuleEditor automatically registers its delegate to receive rowsDidChangeNotification notifications.

