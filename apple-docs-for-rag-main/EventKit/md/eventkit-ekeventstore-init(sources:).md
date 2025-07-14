

- EventKit
- EKEventStore
-  init(sources:) 

Initializer

# init(sources:)

Creates an event store that contains data for the specified sources.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.11+visionOS 1.0+watchOS 9.0+

``` source
init(sources: [EKSource])
```

## Parameters 

`sources`  

An array of sources the event store should contain. This array may include delegate sources.

## Return Value

An event store that contains data for a specific collection of event sources.

## See Also

### Creating event stores

init()

Creates a new event store.

var eventStoreIdentifier: String

The unique identifier for the event store.

