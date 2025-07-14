

- UIKit
- UIDocument
-  stateChangedNotification 

Type Property

# stateChangedNotification

A notification the document object posts when there’s a change in the state of the document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let stateChangedNotification: NSNotification.Name
```

## Discussion

When handling this notification, check the value of the documentState property to see what the new state is, and then proceed accordingly. There’s no `userInfo` dictionary.

