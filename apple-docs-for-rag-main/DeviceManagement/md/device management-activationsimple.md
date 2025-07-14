

- Device Management
-  ActivationSimple 

Object

# ActivationSimple

The declaration to activate a set of configurations.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ActivationSimple
```

## Properties

`Predicate`

`string`

A predicate format string as Apple’s Predicate Programming describes. The activation only installs when the predicate evaluates to `true` or isn’t present.

`StandardConfigurations`

`[string]`

 (Required) 

An array of strings that specify the identifiers of configurations to install. A failure to install one of the configurations doesn’t prevent other configurations from installing.

## Discussion

Specify `com.apple.activation.simple` as the declaration type.

