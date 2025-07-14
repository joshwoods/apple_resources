

- Core Data
- NSPersistentCloudKitContainerEventRequest
-  fetchEvents(matchingFetch:) 

Type Method

# fetchEvents(matchingFetch:)

Creates a fetch request for events that match a specified fetch request from a persistent CloudKit container.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func fetchEvents(matchingFetch fetchRequest: NSFetchRequest) -> Self
```

## Parameters 

`fetchRequest`  

A fetch request to identify matching events.

## Return Value

A request object that fetches persistent CloudKit container events by executing in a managed object context.

## See Also

### Fetching Events

class func fetchEvents(after: Date) -> Self

Creates a fetch request for events after a specified date from a persistent CloudKit container.

class func fetchEvents(after: NSPersistentCloudKitContainer.Event?) -> Self

Creates a fetch request for events that occur after a specified event from a persistent CloudKit container.

class func fetchForEvents() -> NSFetchRequest&lt;any NSFetchRequestResult>

Creates a fetch request for all events in a persistent CloudKit container.

var resultType: NSPersistentCloudKitContainerEventResult.ResultType

The type of result that the request returns.

