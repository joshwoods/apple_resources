

- Core Services
- Apple Events
-  AESizeOfNthItem(\_:\_:\_:\_:) 

Function

# AESizeOfNthItem(\_:\_:\_:\_:)

Gets the data size and descriptor type of the descriptor at a specified position in a descriptor list.

macOS 10.0+

``` source
func AESizeOfNthItem(
    _ theAEDescList: UnsafePointer!,
    _ index: Int,
    _ typeCode: UnsafeMutablePointer!,
    _ dataSize: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list containing the descriptor. See AEDescList.

`index`  

A one-based positive integer indicating the position of the descriptor to get the data size for. `AESizeOfNthItem` returns an error if you pass zero, a negative number, or a value that is out of range.

`typeCode`  

A pointer to a descriptor type. On return, specifies the descriptor type of the descriptor. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataSize`  

A pointer to a size variable. On return, the length (in bytes) of the data in the descriptor.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Getting the Sizes and Descriptor Types of Descriptors

func AESizeOfAttribute(UnsafePointer&lt;AppleEvent>!, AEKeyword, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the size and descriptor type of an Apple event attribute from a descriptor of type `AppleEvent`.

func AESizeOfParam(UnsafePointer&lt;AppleEvent>!, AEKeyword, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the size and descriptor type of an Apple event parameter from a descriptor of type `AERecord` or `AppleEvent`.

