

- XCTest
- XCTApplicationLaunchMetric
-  init() 

Initializer

# init()

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init()
```

## Discussion

If you didn’t start any extended launch tasks using extendLaunchMeasurement(forTaskID:), this metric measures only the time for your app to display its first frame to screen.

## See Also

### Initializers

init(waitUntilResponsive: Bool)

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks, or to display its first frame and wait until the app is responsive.

