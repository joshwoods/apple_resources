

- Foundation
- NSIndexPath
-  getIndexes(\_:) Deprecated

Instance Method

# getIndexes(\_:)

Copies the objects contained in the index path into indexes.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func getIndexes(_ indexes: UnsafeMutablePointer)
```

Deprecated

Use getIndexes(_:range:) instead.

## Parameters 

`indexes`  

Pointer to a C array of objects of size at least the length of the index path. On return, the index path’s indexes.

## Discussion

You must allocate the memory for the C array.

## See Also

### Working with Indexes

func index(atPosition: Int) -> Int

Provides the value at a particular node in the index path.

func getIndexes(UnsafeMutablePointer&lt;Int>, range: NSRange)

Copies the indexes stored in the index path from the positions specified by the position range into the specified indexes.

