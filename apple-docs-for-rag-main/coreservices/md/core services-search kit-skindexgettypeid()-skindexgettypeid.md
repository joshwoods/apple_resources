

- Core Services
- Search Kit
-  SKIndexGetTypeID() 

Function

# SKIndexGetTypeID()

Gets the type identifier for Search Kit indexes.

macOS 10.3+

``` source
func SKIndexGetTypeID() -> CFTypeID
```

## Return Value

A CFTypeID object containing the type identifier for the `SKIndex` opaque type.

## Discussion

Search Kit represents indexes with the SKIndex opaque type. If your code needs to determine whether a particular data type is an index, you can use this function along with the CFGetTypeID(_:) function and perform a comparison.

Never hard-code the index type ID because it can change from one release of macOS to another.

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

func SKIndexClose(SKIndex!)

Closes an index.

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

