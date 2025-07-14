

- Core Services
- Apple Events
-  AECountItems(\_:\_:) 

Function

# AECountItems(\_:\_:)

Counts the number of descriptors in a descriptor list.

macOS 10.0+

``` source
func AECountItems(
    _ theAEDescList: UnsafePointer!,
    _ theCount: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list to count. See AEDescList.

`theCount`  

A pointer to a count variable. On return, the number of descriptors in the specified descriptor list, which can be 0, if the list is empty.

## Return Value

A result code. See Result Codes.

## Discussion

Your application typically counts the descriptors in a descriptor list when it is extracting data from an Apple event. You can use the functions in “Getting Items From Descriptor Lists” to get an individual item from a descriptor list or to iterate through the items.

### Version-Notes

Thread safe starting in OS X v10.2.

