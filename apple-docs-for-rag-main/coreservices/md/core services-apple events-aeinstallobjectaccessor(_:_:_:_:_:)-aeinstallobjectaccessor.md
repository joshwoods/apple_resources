

- Core Services
- Apple Events
-  AEInstallObjectAccessor(\_:\_:\_:\_:\_:) 

Function

# AEInstallObjectAccessor(\_:\_:\_:\_:\_:)

Adds or replaces an entry for an object accessor function to an object accessor dispatch table.

macOS 10.0+

``` source
func AEInstallObjectAccessor(
    _ desiredClass: DescType,
    _ containerType: DescType,
    _ theAccessor: OSLAccessorUPP!,
    _ accessorRefcon: SRefCon!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`desiredClass`  

The object type of the Apple event objects located by this accessor. See DescType.

`containerType`  

The type of the token whose objects are accessed by this accessor. (Token is defined in AEDisposeToken(_:).) The accessor function finds objects in containers specified by tokens of this type. See DescType.

`theAccessor`  

A universal procedure pointer to the object accessor function to install. See OSLAccessorUPP.

`accessorRefcon`  

A reference constant the Apple Event Manager passes to the object accessor function whenever it calls the function. If your object accessor function doesn’t require a reference constant, pass 0 for this parameter. To change the value of the reference constant, you must call `AEInstallObjectAccessor` again.

`isSysHandler`  

Specifies the object accessor dispatch table to add the entry to. Pass `TRUE` to add the entry to the system object accessor dispatch table or `FALSE` to add the entry to your application’s object accessor dispatch table. Use of the system object accessor dispatch table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

The `AEInstallObjectAccessor` function adds or replaces an entry to either the application or system object accessor dispatch table.

### Version-Notes

In macOS, your application can not make an object callback function available to other applications by installing it in a system object accessor dispatch table.

If your Carbon application running in Mac OS 8 or OS 9 installs a system object accessor function in its application heap, rather than in the system heap, you must call AERemoveObjectAccessor(_:_:_:_:) to remove the function before your application terminates.

## See Also

### Getting, Calling, and Removing Object Accessor Functions

func AECallObjectAccessor(DescType, UnsafePointer&lt;AEDesc>!, DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Invokes the appropriate object accessor function for a specific desired type and container type.

func AEGetObjectAccessor(DescType, DescType, UnsafeMutablePointer&lt;OSLAccessorUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, Bool) -> OSErr

Gets an object accessor function from an object accessor dispatch table.

func AERemoveObjectAccessor(DescType, DescType, OSLAccessorUPP!, Bool) -> OSErr

Removes an object accessor function from an object accessor dispatch table.

