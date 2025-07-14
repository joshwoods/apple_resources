

- Metal
- MTLArgument
-  access Deprecated

Instance Property

# access

The argument’s read and/or write access.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var access: MTLBindingAccess { get }
```

## Discussion

This property indicates the type of access qualifiers (read-only, write-only, or read-write) used in the Metal shading language code. For information on possible values, see MTLArgumentAccess.

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

var type: MTLArgumentType

The argument’s resource type.

Deprecated

