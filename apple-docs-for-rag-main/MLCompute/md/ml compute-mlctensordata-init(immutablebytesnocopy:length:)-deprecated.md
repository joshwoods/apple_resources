

- ML Compute
- MLCTensorData
-  init(immutableBytesNoCopy:length:) Deprecated

Initializer

# init(immutableBytesNoCopy:length:)

Creates a tensor data instance with the buffer of immutable data and length of bytes you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    immutableBytesNoCopy bytes: UnsafeRawPointer,
    length: Int
)
```

## Parameters 

`bytes`  

A buffer that contains immutable data.

`length`  

The number of bytes you choose to reference from `bytes`. This number must not exceed the length of `bytes`.

## Discussion

Important

Don’t mutate the underlying bytes in a tensor data instance you create with this initializer. Doing so may result in unexpected behavior.

## See Also

### Creating Tensor Data

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Creates a tensor data instance with the buffer of data and length of bytes you specify.

Deprecated

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: (UnsafeMutableRawPointer, Int) -> Void)

Creates a tensor data instance with a data buffer, byte length, and custom deallocator closure you specify.

Deprecated

