

- Security
-  SecKeychainAddCallback(\_:\_:\_:) Deprecated

Function

# SecKeychainAddCallback(\_:\_:\_:)

Registers your keychain event callback function.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainAddCallback(
    _ callbackFunction: SecKeychainCallback,
    _ eventMask: SecKeychainEventMask,
    _ userContext: UnsafeMutableRawPointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`callbackFunction`  

A pointer to your keychain event callback function, described in SecKeychainCallback.

`eventMask`  

A bit mask indicating the keychain events of which your application wishes to be notified. See SecKeychainEventMask for valid values. Keychain Services tests this mask to determine the keychain events that you wish to receive, and passes these events in the `keychainEvent` parameter of your callback function.

`userContext`  

A pointer to application-defined storage that will be passed to your callback function. Your application can use this to associate any particular call of this function with any particular call of your keychain event callback function.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

It is important to note that the current Foundation or Core Foundation run loop must be active when making this call or the callbacks are not registered. In multithreaded programs, the notifications are registered in the run loop of the thread calling SecKeychainAddCallback(_:_:_:); therefore, delivery of notifications depends on the functioning of that thread’s run loop. If that thread terminates, or is so busy that it doesn’t operate its run loop in a timely manner, notifications will be delayed, and may eventually be dropped without any notification.

For that reason, it is inadvisable for your program to depend on delivery of notifications caused by your own actions (such as depending on receiving a deletion notification before updating a UI view) unless your program is multithreaded and can take notifications on a thread different from the one generating the events.

