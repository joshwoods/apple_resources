

- Core Services
- Search Kit
-  SKSearchCancel(\_:) 

Function

# SKSearchCancel(\_:)

Cancels an asynchronous search request.

macOS 10.4+

``` source
func SKSearchCancel(_ inSearch: SKSearch!)
```

## Parameters 

`inSearch`  

The search object whose associated asynchronous search you want to cancel.

## Discussion

Call this function when you want to cancel an asynchronous search that you initiated with SKSearchCreate(_:_:_:). This function stops the search process if it is still in progress at the time. It does not dispose of the search object (SKSearchRef).

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

## See Also

### Fast Asynchronous Searching

func SKSearchCreate(SKIndex!, CFString!, SKSearchOptions) -> Unmanaged&lt;SKSearch>!

Creates an asynchronous search object for querying an index, and initiates search.

func SKSearchFindMatches(SKSearch!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Float>!, CFTimeInterval, UnsafeMutablePointer&lt;CFIndex>!) -> Bool

Extracts search result information from a search object.

func SKSearchGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit search objects.

