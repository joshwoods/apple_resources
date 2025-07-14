

- Core Image
- CIWarpKernel
-  init(source:) Deprecated

Initializer

# init(source:)

Creates a warp kernel object from the specified kernel source code.

iOS 8.0–12.0DeprecatediPadOS 8.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init?(source string: String)
```

## Parameters 

`string`  

A program in the Core Image Kernel Language that contains a single routine marked using the `kernel` keyword.

## Return Value

A new warp kernel object, or nil if the specified source code does not contain a valid warp kernel routine.

## Discussion

This method is similar to the init(source:) method of the superclass CIKernel, but creates only warp kernels. Use this method when you want to ensure that the type of kernel object returned (if any) is always `CIWarpKernel`.

