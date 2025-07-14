

- Swift
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two types are not identical.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func != (t0: (any Any.Type)?, t1: (any Any.Type)?) -> Bool
```

## Parameters 

`t0`  

A type to compare.

`t1`  

Another type to compare.

## Return Value

`true` if one, but not both, of `t0` and `t1` are `nil`, or if they represent different types; otherwise, `false`.

## See Also

### Querying Runtime Values

struct Mirror

A representation of the substructure and display style of an instance of any type.

struct ObjectIdentifier

A unique identifier for a class instance or metatype.

func type&lt;T, Metatype>(of: T) -> Metatype

Returns the dynamic type of a value.

func == ((any Any.Type)?, (any Any.Type)?) -> Bool

Returns a Boolean value indicating whether two types are identical.

