

- XCTest
- XCTCPUMetric
-  init(application:) 

Initializer

# init(application:)

Creates a CPU metric that records data for the requested app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init(application: XCUIApplication)
```

## Parameters 

`application`  

The application to be tested.

## See Also

### Initializers

init()

Creates a CPU metric that records data for the current process.

init(limitingToCurrentThread: Bool)

Creates a CPU metric that optionally records data only for the current thread.

