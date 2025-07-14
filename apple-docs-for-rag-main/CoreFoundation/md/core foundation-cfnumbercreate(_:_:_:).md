

- Core Foundation
-  CFNumberCreate(\_:\_:\_:) 

Function

# CFNumberCreate(\_:\_:\_:)

Creates a CFNumber object using a specified value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberCreate(
    _ allocator: CFAllocator!,
    _ theType: CFNumberType,
    _ valuePtr: UnsafeRawPointer!
) -> CFNumber!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`theType`  

A constant that specifies the data type of the value to convert. See CFNumberType for a list of possible values.

`valuePtr`  

A pointer to the value for the returned number object.

## Return Value

A new number with the value specified by `valuePtr`. Ownership follows the The Create Rule.

## Discussion

The `theType` parameter is not necessarily preserved when creating a new CFNumber object. The CFNumber object will be created using whatever internal storage type the creation function deems appropriate. Use the function CFNumberGetType(_:) to find out what type the CFNumber object used to store your value.

