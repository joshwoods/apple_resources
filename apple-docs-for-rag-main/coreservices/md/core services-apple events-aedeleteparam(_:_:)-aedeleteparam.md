

- Core Services
- Apple Events
-  AEDeleteParam(\_:\_:) 

Function

# AEDeleteParam(\_:\_:)

Deletes a keyword-specified parameter from an Apple event record.

macOS 10.0+

``` source
func AEDeleteParam(
    _ theAppleEvent: UnsafeMutablePointer!,
    _ theAEKeyword: AEKeyword
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event or Apple event record to delete the parameter from. See AppleEvent.

`theAEKeyword`  

The keyword that specifies the parameter to delete. Some keyword constants are described in Keyword Parameter Constants. See AEKeyword.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Deleting Descriptors

func AEDeleteItem(UnsafeMutablePointer&lt;AEDescList>!, Int) -> OSErr

Deletes a descriptor from a descriptor list, causing all subsequent descriptors to move up one place.

