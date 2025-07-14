

- ML Compute
- MLCTensorData
-  init(bytesNoCopy:length:) Deprecated

Initializer

# init(bytesNoCopy:length:)

Creates a tensor data instance with the buffer of data and length of bytes you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length: Int
)
```

## Parameters 

`bytes`  

A buffer that contains data.

`length`  

The number of bytes you choose to reference from `bytes`. This number must not exceed the length of `bytes`.

## See Also

### Creating Tensor Data

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: (UnsafeMutableRawPointer, Int) -> Void)

Creates a tensor data instance with a data buffer, byte length, and custom deallocator closure you specify.

Deprecated

convenience init(immutableBytesNoCopy: UnsafeRawPointer, length: Int)

Creates a tensor data instance with the buffer of immutable data and length of bytes you specify.

Deprecated

