

- ML Compute
- MLCTensorData
-  init(bytesNoCopy:length:deallocator:) Deprecated

Initializer

# init(bytesNoCopy:length:deallocator:)

Creates a tensor data instance with a data buffer, byte length, and custom deallocator closure you specify.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
convenience init(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length: Int,
    deallocator: @escaping (UnsafeMutableRawPointer, Int) -> Void
)
```

## Parameters 

`bytes`  

A buffer that contains data.

`length`  

The number of bytes you want to reference from `bytes`. This number must not exceed the length of `bytes`.

`deallocator`  

A callback to invoke after the system deallocates the object instance.

## Return Value

A new `MLCTensorData` instance.

## See Also

### Creating Tensor Data

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Creates a tensor data instance with the buffer of data and length of bytes you specify.

Deprecated

convenience init(immutableBytesNoCopy: UnsafeRawPointer, length: Int)

Creates a tensor data instance with the buffer of immutable data and length of bytes you specify.

Deprecated

