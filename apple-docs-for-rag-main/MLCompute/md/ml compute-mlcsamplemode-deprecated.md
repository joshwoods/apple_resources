

- ML Compute
-  MLCSampleMode Deprecated

Enumeration

# MLCSampleMode

A sampling mode for an upsample layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCSampleMode
```

## Topics

### Enumeration Cases

case nearest

case linear

var debugDescription: String

A textual description of the sample mode, suitable for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Upsample Layers

convenience init?(shape: [Int])

Creates an upsample layer with the shape you specify.

Deprecated

convenience init?(shape: [Int], sampleMode: MLCSampleMode, alignsCorners: Bool)

Creates an upsample layer with the shape, upsampling algorithm, and corner alignment option you specify.

Deprecated

