

- Metal
- MTLArgument
-  type Deprecated

Instance Property

# type

The argument’s resource type.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var type: MTLArgumentType { get }
```

## Discussion

This property indicates which type of resource is used (buffer, texture, sampler, or threadgroup memory) in the shading language code. For information on possible values, see MTLArgumentType.

## See Also

### Describing the Argument

var name: String

The name of the argument.

Deprecated

var isActive: Bool

A Boolean that indicates whether the compiled function uses the argument.

Deprecated

var index: Int

The index in the argument table that corresponds to the function argument.

Deprecated

var access: MTLBindingAccess

The argument’s read and/or write access.

Deprecated

