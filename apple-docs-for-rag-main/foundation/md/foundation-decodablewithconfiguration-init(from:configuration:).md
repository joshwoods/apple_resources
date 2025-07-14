

- Foundation
- DecodableWithConfiguration
-  init(from:configuration:) 

Initializer

# init(from:configuration:)

Creates a new instance by retrieving the instance’s data from the specified decoder with help from the provided configuration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    from decoder: any Decoder,
    configuration: Self.DecodingConfiguration
) throws
```

**Required**

## Parameters 

`decoder`  

The decoder to read data from.

`configuration`  

A decoding configuration instance that provides additional information necessary for decoding.

