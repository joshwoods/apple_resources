

- ARKit
- ARSessionObserver
-  session(\_:didOutputCollaborationData:) 

Instance Method

# session(\_:didOutputCollaborationData:)

Provides information for nearby users about your perspective in the environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didOutputCollaborationData data: ARSession.CollaborationData
)
```

## Parameters 

`session`  

The app’s collaborative session.

`data`  

The information to share with participants.

## Discussion

The data parameter contains information about your perspective in the physical environment. When ARKit invokes this function, send the `data` object to nearby users. The users update their session with your data to gain your app’s model of the physical environment in addition to their own. For more information, see isCollaborationEnabled.

For an example app that implements this callback, see Creating a collaborative session.

