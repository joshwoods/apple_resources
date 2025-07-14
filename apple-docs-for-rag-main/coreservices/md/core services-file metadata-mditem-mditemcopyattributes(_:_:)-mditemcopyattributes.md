

- Core Services
- File Metadata
- MDItem
-  MDItemCopyAttributes(\_:\_:) 

Function

# MDItemCopyAttributes(\_:\_:)

Returns the values of the specified attributes in the metadata item.

macOS 10.4+

``` source
func MDItemCopyAttributes(
    _ item: MDItem!,
    _ names: CFArray!
) -> CFDictionary!
```

## Parameters 

`item`  

The item to be queried.

`names`  

A CFArray containing the names of the requested attributes.

## Return Value

A CFDictionary containing keys for the requested attribute names, and the corresponding values. If an attribute does not exist, or the attribute is unreadable, there will be no key-value pair for it in the dictionary. Returns `NULL` on failure.

## See Also

### Retrieving Metadata Attributes 

func MDItemCopyAttribute(MDItem!, CFString!) -> CFTypeRef!

Returns the value of the specified attribute in the metadata item.

func MDItemCopyAttributeNames(MDItem!) -> CFArray!

Returns an array containing the attribute names existing in the metadata item.

