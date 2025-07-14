

- Core Services
- Search Kit
-  SKSearchFindMatches(\_:\_:\_:\_:\_:\_:) 

Function

# SKSearchFindMatches(\_:\_:\_:\_:\_:\_:)

Extracts search result information from a search object.

macOS 10.4+

``` source
func SKSearchFindMatches(
    _ inSearch: SKSearch!,
    _ inMaximumCount: CFIndex,
    _ outDocumentIDsArray: UnsafeMutablePointer!,
    _ outScoresArray: UnsafeMutablePointer!,
    _ maximumTime: CFTimeInterval,
    _ outFoundCount: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`inSearch`  

A reference to a search object (SKSearchRef) previously created with `SKSearchCreate(_:_:_:)`.

`inMaximumCount`  

The maximum number of items to find. For each item found, `SKSearchFindMatches(_:_:_:_:_:_:)` places the associated document ID into the `outDocumentIDsArray` array. Specify an `inMaximumCount` of 0 to find as many items as possible within `maximumTime`.

`outDocumentIDsArray`  

On input, a pointer to an array for document IDs. On output, points to points to the previously allocated array, which now contains the found document IDs. The size of this array must be equal to `inMaximumCount`.

`outScoresArray`  

On input, a pointer to an array for scores. On output, points to the previously allocated array, which now contains relevance scores for the found items. The size of this array, if not `NULL`, must be equal to `inMaximumCount`. Can be `NULL` on input, provided that your application doesn’t need this information. Search Kit does not normalize relevance scores, so they can be very large.

`maximumTime`  

The maximum number of seconds before this function returns, whether or not `inMaximumCount` items have been found. Setting maximumTime to 0 tells the search to return quickly

`outFoundCount`  

On input, a pointer to a CFIndex object that will hold the number of items found. On output, points to the CFIndex object that now contains the actual number of items found.

## Return Value

A logical value indicating whether the search is still in progress. Returns false when the search is exhausted.

## Discussion

The `SKSearchFindMatches(_:_:_:_:_:_:)` extracts results from a find operation initiated by a search object (SKSearchRef).

This function provides results to its output parameters simply in the order in which they are found. This reduces latency to support search-as-you-type functionality. Larger scores mean greater relevance.

You can call this function on a search object repeatedly to get additional sets of search results. For example, if you call this function twice with an `inMaximumCount` value of 10, the first call will put the first 10 items found into the output arrays and the second call will put the second 10 items found into the output arrays.

Applications are free to display relevance scores in any appropriate manner. One simple way is to divide each relevance score by the largest number returned to get relevance numbers scaled linearly from 0.0 to 1.0. Search Kit does not scale the relevance scores for you, because you may want to combine the scores from several calls on a search object or the scores from calls to more than one search object.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

Before invoking a search, call SKIndexFlush(_:) on all indexes you will query to ensure that updates to the indexes have been flushed to disk.

## See Also

### Fast Asynchronous Searching

func SKSearchCreate(SKIndex!, CFString!, SKSearchOptions) -> Unmanaged&lt;SKSearch>!

Creates an asynchronous search object for querying an index, and initiates search.

func SKSearchCancel(SKSearch!)

Cancels an asynchronous search request.

func SKSearchGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit search objects.

