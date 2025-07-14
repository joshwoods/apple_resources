

- Metal
- MTLArgument
-  index Deprecated

Instance Property

# index

The index in the argument table that corresponds to the function argument.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var index: Int { get }
```

## Discussion

A command encoder (MTLComputeCommandEncoder or MTLRenderCommandEncoder) specifies the index in the corresponding argument table. For example, an app can call the setTexture(_:index:) method of MTLComputeCommandEncoder to specify an index in the texture argument table for a MTLTexture object that is used as an argument of a compute function.

## See Also

### Describing the Argument

var name: String

The name of the argument.

Deprecated

var isActive: Bool

A Boolean that indicates whether the compiled function uses the argument.

Deprecated

var type: MTLArgumentType

The argument’s resource type.

Deprecated

var access: MTLBindingAccess

The argument’s read and/or write access.

Deprecated

