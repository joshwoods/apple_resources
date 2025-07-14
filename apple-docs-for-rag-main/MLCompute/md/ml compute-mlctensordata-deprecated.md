

- ML Compute
-  MLCTensorData Deprecated

Class

# MLCTensorData

An encapsulation of the memory that tensor data uses.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCTensorData
```

## Overview

Important

A tensor data instance doesn’t take ownership of the `bytes` pointer and therefore won’t free it upon deallocation.

## Topics

### Creating Tensor Data

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Creates a tensor data instance with the buffer of data and length of bytes you specify.

convenience init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: (UnsafeMutableRawPointer, Int) -> Void)

Creates a tensor data instance with a data buffer, byte length, and custom deallocator closure you specify.

convenience init(immutableBytesNoCopy: UnsafeRawPointer, length: Int)

Creates a tensor data instance with the buffer of immutable data and length of bytes you specify.

### Inspecting Tensor Data

var bytes: UnsafeMutableRawPointer

A buffer that conains data.

var length: Int

The number of bytes you choose to hold for this tensor data instance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating Tensors with Descriptors

convenience init(descriptor: MLCTensorDescriptor)

Creates a tensor without data, using the descriptor you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, data: MLCTensorData)

Creates a tensor with the descriptor and data you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, fillWithData: NSNumber)

Creates a tensor with the descriptor and scalar value you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the descriptor and random initializer type you specify.

Deprecated

class MLCTensorDescriptor

A configuration object you use to create a tensor.

Deprecated

enum MLCDataType

A tensor data type.

Deprecated

enum MLCRandomInitializerType

An initializer type you use to create a tensor with random data.

Deprecated

