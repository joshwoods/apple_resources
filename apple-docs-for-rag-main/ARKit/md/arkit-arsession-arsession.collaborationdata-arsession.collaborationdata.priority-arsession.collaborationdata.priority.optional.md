

- ARKit
- ARSession
- ARSession.CollaborationData
- ARSession.CollaborationData.Priority
-  ARSession.CollaborationData.Priority.optional 

Case

# ARSession.CollaborationData.Priority.optional

A priority that indicates that collaboration can continue without this data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
case optional
```

## Discussion

ARKit sets the data priority to ARSession.CollaborationData.Priority.optional when the data is important and time-sensitive but the session can continue if it’s not received.

