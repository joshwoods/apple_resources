

- Core Location
- CLBackgroundActivitySession
-  invalidate() 

Instance Method

# invalidate()

Invalidates the background activity session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+watchOS 10.0+

``` source
final func invalidate()
```

## Discussion

This method ends the session immediately. The system terminates any UI that displays a visual indication to this background session. After you invalidate a session, it can’t become active again and you need to create a new session to begin receiving updates again.

