

- EventKit
- EKEventStore
-  source(withIdentifier:) 

Instance Method

# source(withIdentifier:)

Locates an event source with the specified identifier.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func source(withIdentifier identifier: String) -> EKSource?
```

## Parameters 

`identifier`  

The source’s unique identifier.

## Return Value

The source with the specified identifier, or `nil` if the source isn’t found.

## See Also

### Accessing account sources

var sources: [EKSource]

An unordered array of objects that represent accounts that contain calendars.

var delegateSources: [EKSource]

The event sources delegated to the person using your app.

