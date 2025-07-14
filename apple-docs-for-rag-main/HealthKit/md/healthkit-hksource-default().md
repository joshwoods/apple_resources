

- HealthKit
- HKSource
-  default() 

Type Method

# default()

Returns a source object for the current app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func `default`() -> HKSource
```

## Return Value

A source object for the current app.

## Discussion

You can access the source object for the current app directly using this methods. To access other sources, use a source query or similar approach.

