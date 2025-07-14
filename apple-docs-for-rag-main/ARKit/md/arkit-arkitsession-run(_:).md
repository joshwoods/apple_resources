

- ARKit
- ARKitSession
-  run(\_:) 

Instance Method

# run(\_:)

Runs a session with the data providers you supply.

visionOS 1.0+

``` source
final func run(_ dataProviders: [any DataProvider]) async throws
```

## Parameters 

`dataProviders`  

The providers that supply data during this session.

## Discussion

If you call this method without previously calling the requestAuthorization(for:) method, and if any of the data providers you supply require authorization, the system prompts the user for authorization when you call run(_:). If you call this method on an already-running session, ARKit stops the previous providers unless they’re also in the new array of providers.

This method either throws an ARKitSession.Error or asserts when there’s a problem with the data providers you supply. Potential problems include:

- Passing a data provider that’s already in use in another session

- Passing a data provider that’s stopped

- Passing a data provider that’s not supported in the current context, such as in Simulator

When this method throws an error, its session stops all of the associated data providers.

## See Also

### Starting and stopping a session

convenience init()

Creates a new session.

func stop()

Stops all data providers running in this session.

struct Error

An error that might occur when running data providers on an ARKit session.

