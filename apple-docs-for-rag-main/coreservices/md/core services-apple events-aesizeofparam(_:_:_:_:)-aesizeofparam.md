

- Core Services
- Apple Events
-  AESizeOfParam(\_:\_:\_:\_:) 

Function

# AESizeOfParam(\_:\_:\_:\_:)

Gets the size and descriptor type of an Apple event parameter from a descriptor of type `AERecord` or `AppleEvent`.

macOS 10.0+

``` source
func AESizeOfParam(
    _ theAppleEvent: UnsafePointer!,
    _ theAEKeyword: AEKeyword,
    _ typeCode: UnsafeMutablePointer!,
    _ dataSize: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to get the parameter data from. See AppleEvent.

`theAEKeyword`  

The keyword that specifies the desired parameter. Some keyword parameter constants are described in Keyword Parameter Constants. See AEKeyword.

`typeCode`  

A pointer to a descriptor type. On return, specifies the descriptor type of the Apple event parameter. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataSize`  

A pointer to a size variable. On return, the length, in bytes, of the data in the Apple event parameter.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Getting the Sizes and Descriptor Types of Descriptors

func AESizeOfAttribute(UnsafePointer&lt;AppleEvent>!, AEKeyword, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the size and descriptor type of an Apple event attribute from a descriptor of type `AppleEvent`.

func AESizeOfNthItem(UnsafePointer&lt;AEDescList>!, Int, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the data size and descriptor type of the descriptor at a specified position in a descriptor list.

