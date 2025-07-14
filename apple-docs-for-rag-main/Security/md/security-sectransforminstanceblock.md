

- Security
-  SecTransformInstanceBlock 

Type Alias

# SecTransformInstanceBlock

A block that you return from a transform creation function.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SecTransformInstanceBlock = () -> Unmanaged?
```

## Return Value

A an error object if an error occurred.

## Discussion

You return a block of this type from the custom transform creation function of type SecTransformCreateFP that you register with the SecTransformRegister(_:_:_:) function.

