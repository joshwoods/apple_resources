

- CarKey
- CarKeyRemoteControlSession
-  end() 

Instance Method

# end()

Ends the session and stops the delivery of notifications for all vehicles in the session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func end() throws
```

## Discussion

When you no longer need to access the vehicle information, call this method to end the session. If the session isn’t currently active when you call this method, it throws an error.

The system automatically ends a session when your app enters the background. Upon reentering the foreground, you must create a new session to communicate with your vehicle again.

