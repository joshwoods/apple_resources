

- MapKit
- MKLocalSearch
- MKLocalSearch.Request
-  init(completion:) 

Initializer

# init(completion:)

Creates and returns a search request based on the specified search completion data.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
init(completion: MKLocalSearchCompletion)
```

## Parameters 

`completion`  

A search completion object that MapKit obtains from an MKLocalSearchCompleter object. The search request uses the provided object to set the value of the naturalLanguageQuery property.

## Return Value

An initialized search request.

## Discussion

Use this method when initializing your object from MKLocalSearchCompleter objects. You don’t need to use this method if you intend to provide the search string and region information yourself.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a local search request

init()

Creates a local search request.

