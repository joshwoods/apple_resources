

- Core Services
- Apple Events
-  AEDeleteItem(\_:\_:) 

Function

# AEDeleteItem(\_:\_:)

Deletes a descriptor from a descriptor list, causing all subsequent descriptors to move up one place.

macOS 10.0+

``` source
func AEDeleteItem(
    _ theAEDescList: UnsafeMutablePointer!,
    _ index: Int
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list containing the descriptor to delete. See AEDescList.

`index`  

A one-based positive integer indicating the position of the descriptor to delete. `AEDeleteItem` returns an error if you pass zero, a negative number, or a value that is out of range.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Deleting Descriptors

func AEDeleteParam(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword) -> OSErr

Deletes a keyword-specified parameter from an Apple event record.

