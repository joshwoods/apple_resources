

- Core Services
- Search Kit
-  SKIndexClose(\_:) 

Function

# SKIndexClose(\_:)

Closes an index.

macOS 10.4+

``` source
func SKIndexClose(_ inIndex: SKIndex!)
```

## Parameters 

`inIndex`  

The index to close.

## Discussion

When your application no longer needs an index that it has opened or created, call `SKIndexClose(_:)`. Calling this function is equivalent to calling CFRelease on an index.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

## See Also

### Creating, Opening, and Closing Indexes

func SKIndexCreateWithURL(CFURL!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index in a file whose location is specified with a CFURL object.

func SKIndexCreateWithMutableData(CFMutableData!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index stored in a `CFMutableDataRef` object.

func SKIndexOpenWithData(CFData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching only.

func SKIndexOpenWithMutableData(CFMutableData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching and updating.

func SKIndexOpenWithURL(CFURL!, CFString!, Bool) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index stored in a file whose location is specified with a CFURL object.

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

