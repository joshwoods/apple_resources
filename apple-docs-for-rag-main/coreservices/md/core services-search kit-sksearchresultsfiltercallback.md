

- Core Services
- Search Kit
-  SKSearchResultsFilterCallBack 

Type Alias

# SKSearchResultsFilterCallBack

Deprecated. Use `SKSearchCreate` and `SKSearchFindMatches` instead, which do not use a callback.

Mac Catalyst 13.0+macOS 10.3+

``` source
typealias SKSearchResultsFilterCallBack = (SKIndex?, SKDocument?, UnsafeMutableRawPointer?) -> DarwinBoolean
```

## Parameters 

`inIndex`  

The index you are searching.

`inDocument`  

The document URL object within the index you are searching.

`inContext`  

An application-specified context which you set when calling SKSearchResultsCreateWithQuery or SKSearchResultsCreateWithDocuments.

## Return Value

A Boolean value of `true` for a successful search hit, or `false` otherwise.

## Discussion

Deprecated. Defines a pointer to a search-results filtering callback function for hit testing and processing during a search. Use this callback function to perform custom filtering on the search hits returned by the SKSearchResultsCreateWithQuery and SKSearchResultsCreateWithDocuments functions. Return `true` to keep this document URL object (SKDocumentRef) in the results, `false` to filter it out.

