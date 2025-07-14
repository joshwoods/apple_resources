

- Metal
- MTLArgument
-  isActive Deprecated

Instance Property

# isActive

A Boolean that indicates whether the compiled function uses the argument.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var isActive: Bool { get }
```

## Discussion

When you create the MTLFunction object, Metal statically determines whether the function uses the argument. If true, you must provide a value for this argument when you encode a command that calls this function. If false, the function doesn’t use the argument, and you can ignore it.

## See Also

### Describing the Argument

var name: String

The name of the argument.

Deprecated

var index: Int

The index in the argument table that corresponds to the function argument.

Deprecated

var type: MTLArgumentType

The argument’s resource type.

Deprecated

var access: MTLBindingAccess

The argument’s read and/or write access.

Deprecated

