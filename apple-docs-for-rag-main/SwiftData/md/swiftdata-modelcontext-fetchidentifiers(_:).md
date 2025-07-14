

- SwiftData
- ModelContext
-  fetchIdentifiers(\_:) 

Instance Method

# fetchIdentifiers(\_:)

Returns an array of persistent identifiers, where each identifier represents a single model that satisfies the criteria of the specified fetch descriptor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
func fetchIdentifiers(_ descriptor: FetchDescriptor) throws -> [PersistentIdentifier] where T : PersistentModel
```

## Parameters 

`descriptor`  

A fetch descriptor that provides the configuration for the fetch.

## Return Value

The array of persistent identifiers. If no models match the descriptor’s criteria, the array is empty.

## See Also

### Fetching only persistent identifiers

func fetchIdentifiers&lt;T>(FetchDescriptor&lt;T>, batchSize: Int) throws -> FetchResultsCollection&lt;PersistentIdentifier>

Returns a collection of persistent identifiers, in batches, where each identifier represents a single model that satisfies the criteria of the specified fetch descriptor.

