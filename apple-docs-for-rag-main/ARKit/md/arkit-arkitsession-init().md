

- ARKit
- ARKitSession
-  init() 

Initializer

# init()

Creates a new session.

visionOS 1.0+

``` source
convenience init()
```

## Discussion

ARKit stops sessions when they’re deinitialized.

## See Also

### Starting and stopping a session

func run([any DataProvider]) async throws

Runs a session with the data providers you supply.

func stop()

Stops all data providers running in this session.

struct Error

An error that might occur when running data providers on an ARKit session.

