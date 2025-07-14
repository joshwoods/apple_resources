

- Core Services
- Apple Events
-  AEPutAttributeDesc(\_:\_:\_:) 

Function

# AEPutAttributeDesc(\_:\_:\_:)

Adds a descriptor and a keyword to an Apple event as an attribute.

macOS 10.0+

``` source
func AEPutAttributeDesc(
    _ theAppleEvent: UnsafeMutablePointer!,
    _ theAEKeyword: AEKeyword,
    _ theAEDesc: UnsafePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to add an attribute to. See the AppleEvent data type.

`theAEKeyword`  

The keyword for the attribute to add. If the Apple event already includes an attribute with this keyword, the attribute is replaced.

Some keyword constants are described in Keyword Attribute Constants.

See AEKeyword.

`theAEDesc`  

A pointer to the descriptor to assign to the attribute. The descriptor type of the specified descriptor should match the defined descriptor type for that attribute. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

The `AEPutAttributeDesc` function takes a descriptor and a keyword and adds them to an Apple event as an attribute. If the descriptor type required for the attribute is different from the descriptor type of the descriptor, the Apple Event Manager attempts to coerce the descriptor into the required type, with one exception: the Apple Event Manager does not attempt to coerce the data for an address attribute, thereby allowing applications to use their own address types.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Adding Parameters and Attributes to Apple Events and Apple Event Records

func AEPutAttributePtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Adds a pointer to data, a descriptor type, and a keyword to an Apple event as an attribute.

func AEPutParamDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Inserts a descriptor and a keyword into an Apple event or Apple event record as an Apple event parameter.

func AEPutParamPtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data, a descriptor type, and a keyword into an Apple event or Apple event record as an Apple event parameter.

