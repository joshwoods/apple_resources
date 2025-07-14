

- Core Spotlight
- CSSearchQuery
-  CSSearchQuery.Results 

Structure

# CSSearchQuery.Results

An asynchronous sequence that contains the results that match the query string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct Results
```

## Discussion

A `CSSearchQuery/Results-swift.struct` structure contains the results of a query. Fetch this structure from the results property of your query object to execute the query automatically and begin the delivery of the results. Use each instance of the structure to get the details for a single result.

For more information about how to use this structure, see the results property.

## Topics

### Structures

struct Item

struct Iterator

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Executing the query automatically

var results: CSSearchQuery.Results

The results that match the current query string.

