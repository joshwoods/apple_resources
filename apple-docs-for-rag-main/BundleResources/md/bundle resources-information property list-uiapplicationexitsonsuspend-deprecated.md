

- Bundle Resources
- Information Property List
-  UIApplicationExitsOnSuspend Deprecated

Property List Key

# UIApplicationExitsOnSuspend

A Boolean value indicating whether the app terminates, rather than moves to the background, when the app quits.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0+watchOS 2.0–6.0Deprecated

Deprecated

The system now automatically suspends apps leaving the foreground when they don’t require background execution. For more information, see About the background execution sequence.

## Details 

Name  
Application does not run in background

Type  

boolean

## See Also

### Termination

LSGetAppDiedEvents

A Boolean value indicating whether the app is notified when a child process dies.

**Name:** Application should get App Died events

NSSupportsSuddenTermination

A Boolean value indicating whether the system may terminate the app to log out or shut down more quickly.

**Name:** Application can be killed immediately after launch

