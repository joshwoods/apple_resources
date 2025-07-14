

- AppKit
- NSDocument
-  updateUserActivityState(\_:) 

Instance Method

# updateUserActivityState(\_:)

Updates the state of the given user activity.

macOS 10.10+

``` source
@MainActor
func updateUserActivityState(_ activity: NSUserActivity)
```

## Parameters 

`activity`  

The user activity to be updated.

## Discussion

The default implementation of this method puts the document’s fileURL into the NSUserActivity object’s userInfo dictionary with the NSUserActivityDocumentURLKey. NSDocument automatically sets the needsSave property of the NSUserActivity to true when the fileURL changes.

## See Also

### Related Documentation

class NSDocument

An abstract class that defines the interface for macOS documents.

### Supporting User Activities

var userActivity: NSUserActivity?

An object that encapsulates a user activity the document supports.

let NSUserActivityDocumentURLKey: String

The key that identifies the document associated with a user activity.

