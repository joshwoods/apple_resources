

- AppKit
- NSDocumentController
-  autosavingDelay 

Instance Property

# autosavingDelay

The time interval (in seconds) for periodic autosaving.

macOS

``` source
@MainActor
var autosavingDelay: TimeInterval { get set }
```

## Discussion

A value of 0 indicates that periodic autosaving should not be done at all. The `NSDocumentController` object uses this number as the amount of time to wait between detecting that a document has unautosaved changes and sending the document an autosave(withDelegate:didAutosave:contextInfo:) message. The default value is `0`.

