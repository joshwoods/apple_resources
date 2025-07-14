

- Core Services
- Search Kit
-  SKSearchGetTypeID() 

Function

# SKSearchGetTypeID()

Gets the type identifier for Search Kit search objects.

macOS 10.4+

``` source
func SKSearchGetTypeID() -> CFTypeID
```

## Return Value

A CFTypeID object containing the type identifier for the SKSearch opaque type.

## Discussion

Search Kit represents searches with search objects (SKSearch opaque types). If your code needs to determine whether a particular data type is a search object, you can use this function along with the CFGetTypeID(_:) function and perform a comparison.

Never hard-code the search type ID because it can change from one release of macOS to another.

## See Also

### Fast Asynchronous Searching

func SKSearchCreate(SKIndex!, CFString!, SKSearchOptions) -> Unmanaged&lt;SKSearch>!

Creates an asynchronous search object for querying an index, and initiates search.

func SKSearchFindMatches(SKSearch!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Float>!, CFTimeInterval, UnsafeMutablePointer&lt;CFIndex>!) -> Bool

Extracts search result information from a search object.

func SKSearchCancel(SKSearch!)

Cancels an asynchronous search request.

