

- Core Foundation
-  CFXMLCreateStringByEscapingEntities(\_:\_:\_:) 

Function

# CFXMLCreateStringByEscapingEntities(\_:\_:\_:)

Given a CFString object containing XML source with unescaped entities, returns a string with specified XML entities escaped.

macOS

``` source
func CFXMLCreateStringByEscapingEntities(
    _ allocator: CFAllocator!,
    _ string: CFString!,
    _ entitiesDictionary: CFDictionary!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`string`  

Any CFString object that may contain XML source. This function translates any substring that is mapped to an entity in `entitiesDictionary` to the specified entity.

`entitiesDictionary`  

Specifies the entities to be replaced. Dictionary keys should be the entity names (for example, “para” for ¶), and the values should be CFString objects containing the expansion. Pass `NULL` to indicate no entities other than the standard five.

## Return Value

A CFString object derived from `string` with substrings identified in `entitiesDictionary` escaped to their corresponding entities. Ownership follows the The Create Rule.

## Discussion

The standard five predefined entities are automatically supported.

As an example of using this function, say you apply this function to string “Refer to ¶ 5 of the contract” with a key of “para” mapped to “¶” in `entitiesDictionary`. The resulting string is “Refer to ¶ 5 of the contract”.

Note

Currently, only the standard predefined entities are supported; passing `NULL` for `entitiesDictionary` is sufficient.

## See Also

### CFXMLTree Miscellaneous Functions

func CFXMLCreateStringByUnescapingEntities(CFAllocator!, CFString!, CFDictionary!) -> CFString!

Given a CFString object containing XML source with escaped entities, returns a string with specified XML entities unescaped.

