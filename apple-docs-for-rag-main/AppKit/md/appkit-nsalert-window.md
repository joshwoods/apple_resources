

- AppKit
- NSAlert
-  window 

Instance Property

# window

The app-modal panel or document-modal sheet that corresponds to the alert.

macOS

``` source
@MainActor
var window: NSWindow { get }
```

## Discussion

The alert’s window is of type NSPanel. Use this property when you want to dismiss an alert created with the beginSheetModal(for:completionHandler:) method within that method’s completion handler block.

