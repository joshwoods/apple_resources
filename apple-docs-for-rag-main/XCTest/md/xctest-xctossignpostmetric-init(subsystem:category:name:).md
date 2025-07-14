

- XCTest
- XCTOSSignpostMetric
-  init(subsystem:category:name:) 

Initializer

# init(subsystem:category:name:)

Creates a metric to record a specific signpost.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    subsystem: String,
    category: String,
    name: String
)
```

## Parameters 

`subsystem`  

The OSLog subsystem that logs the signpost events.

`category`  

The log category for the logged signpost events.

`name`  

The name of the signpost.

## Discussion

Create an `XCTOSSignpostMetric` that records the time that elapses between the beginning and end of the named signpost in a particular log subsystem and category.

