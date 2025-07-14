

- Core Services
- File Metadata
- MDItem
-  MDItemCopyAttribute(\_:\_:) 

Function

# MDItemCopyAttribute(\_:\_:)

Returns the value of the specified attribute in the metadata item.

macOS 10.4+

``` source
func MDItemCopyAttribute(
    _ item: MDItem!,
    _ name: CFString!
) -> CFTypeRef!
```

## Parameters 

`item`  

The item to be queried.

`name`  

The name of the requested attribute.

## Return Value

A CFTypeRef, or `NULL` if there was a failure reading the attribute or the attribute does not exist.

## See Also

### Retrieving Metadata Attributes 

func MDItemCopyAttributes(MDItem!, CFArray!) -> CFDictionary!

Returns the values of the specified attributes in the metadata item.

func MDItemCopyAttributeNames(MDItem!) -> CFArray!

Returns an array containing the attribute names existing in the metadata item.

