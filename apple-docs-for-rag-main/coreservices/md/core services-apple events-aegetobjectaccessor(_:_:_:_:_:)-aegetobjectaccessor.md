

- Core Services
- Apple Events
-  AEGetObjectAccessor(\_:\_:\_:\_:\_:) 

Function

# AEGetObjectAccessor(\_:\_:\_:\_:\_:)

Gets an object accessor function from an object accessor dispatch table.

macOS 10.0+

``` source
func AEGetObjectAccessor(
    _ desiredClass: DescType,
    _ containerType: DescType,
    _ accessor: UnsafeMutablePointer!,
    _ accessorRefcon: UnsafeMutablePointer!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`desiredClass`  

The object class of the Apple event objects located by the object accessor function to get. Pass the value `typeWildCard` to get an object accessor function whose entry in an object accessor dispatch table specifies `typeWildCard` as the object class. Pass the value `cProperty` to get an object accessor function whose entry in an object accessor dispatch table specifies `cProperty` (a constant used to specify a property of any object class). Some other possible values are defined in Object Class ID Constants. See DescType.

`containerType`  

The descriptor type of the token that identifies the container for the objects located by the requested accessor function. (Token is defined in AEDisposeToken(_:).) Pass the value `typeWildCard` to get an object accessor function whose entry in an object accessor dispatch table specifies `typeWildCard` as the descriptor type of the token used to specify the container type. See DescType.

`accessor`  

A universal procedure pointer. On return, a pointer to the requested object accessor function, if an object accessor dispatch table entry exists that exactly matches the values supplied in the parameters `desiredClass` and `containerType`. See OSLAccessorUPP.

`accessorRefcon`  

A pointer to a reference constant. On return, points to the reference constant from the object accessor dispatch table entry for the specified object accessor function. The reference constant may have a value of 0.

`isSysHandler`  

Specifies the object accessor dispatch table to get the object accessor function from. Pass `TRUE` to get the object accessor function from the system object accessor dispatch table or `FALSE` to get the object accessor function from your application’s object accessor dispatch table. Use of the system object accessor dispatch table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

Calling `AEGetObjectAccessor` does not remove the object accessor function from an object accessor dispatch table.

### Version-Notes

In macOS, your application can not make an object callback function available to other applications by installing it in a system object accessor dispatch table.

## See Also

### Getting, Calling, and Removing Object Accessor Functions

func AECallObjectAccessor(DescType, UnsafePointer&lt;AEDesc>!, DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Invokes the appropriate object accessor function for a specific desired type and container type.

func AEInstallObjectAccessor(DescType, DescType, OSLAccessorUPP!, SRefCon!, Bool) -> OSErr

Adds or replaces an entry for an object accessor function to an object accessor dispatch table.

func AERemoveObjectAccessor(DescType, DescType, OSLAccessorUPP!, Bool) -> OSErr

Removes an object accessor function from an object accessor dispatch table.

