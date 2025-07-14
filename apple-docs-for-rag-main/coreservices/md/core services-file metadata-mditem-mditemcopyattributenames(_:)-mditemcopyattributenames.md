

- Core Services
- File Metadata
- MDItem
-  MDItemCopyAttributeNames(\_:) 

Function

# MDItemCopyAttributeNames(\_:)

Returns an array containing the attribute names existing in the metadata item.

macOS 10.4+

``` source
func MDItemCopyAttributeNames(_ item: MDItem!) -> CFArray!
```

## Parameters 

`item`  

The item to be queried.

## Return Value

A CFArray of CFString attribute names, or `NULL` on failure.

## See Also

### Retrieving Metadata Attributes 

func MDItemCopyAttribute(MDItem!, CFString!) -> CFTypeRef!

Returns the value of the specified attribute in the metadata item.

func MDItemCopyAttributes(MDItem!, CFArray!) -> CFDictionary!

Returns the values of the specified attributes in the metadata item.

