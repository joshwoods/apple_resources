

- ARKit
- ARKitSession
-  stop() 

Instance Method

# stop()

Stops all data providers running in this session.

visionOS 1.0+

``` source
final func stop()
```

## Discussion

ARKit also automatically stops sessions when they’re deinitialized.

## See Also

### Starting and stopping a session

convenience init()

Creates a new session.

func run([any DataProvider]) async throws

Runs a session with the data providers you supply.

struct Error

An error that might occur when running data providers on an ARKit session.

