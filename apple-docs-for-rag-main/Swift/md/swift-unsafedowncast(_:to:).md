

- Swift
-  unsafeDowncast(\_:to:) 

Function

# unsafeDowncast(\_:to:)

Returns the given instance cast unconditionally to the specified type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unsafeDowncast(
    _ x: AnyObject,
    to type: T.Type
) -> T where T : AnyObject
```

## Parameters 

`x`  

An instance to cast to type `T`.

`type`  

The type `T` to which `x` is cast.

## Return Value

The instance `x`, cast to type `T`.

## Discussion

The instance passed as `x` must be an instance of type `T`.

Use this function instead of `unsafeBitcast(_:to:)` because this function is more restrictive and still performs a check in debug builds. In -O builds, no test is performed to ensure that `x` actually has the dynamic type `T`.

Warning

This function trades safety for performance. Use `unsafeDowncast(_:to:)` only when you are confident that `x is T` always evaluates to `true`, and only after `x as! T` has proven to be a performance problem.

## See Also

### Instance Casting

func unsafeBitCast&lt;T, U>(T, to: U.Type) -> U

Returns the bits of the given instance, interpreted as having the specified type.

