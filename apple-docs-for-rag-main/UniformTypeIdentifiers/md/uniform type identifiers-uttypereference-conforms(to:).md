

- Uniform Type Identifiers
- UTTypeReference
-  conforms(to:) 

Instance Method

# conforms(to:)

Returns a Boolean value that indicates whether a type conforms to the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func conforms(to type: UTType) -> Bool
```

## Parameters 

`type`  

An UTType instance.

## Return Value

true if the type directly or indirectly conforms to `type`, or if it’s equal to `type`.

## See Also

### Checking a type’s relationship to another type

var supertypes: Set&lt;UTType>

The set of types the type directly or indirectly conforms to.

func isSubtype(of: UTType) -> Bool

Returns a Boolean value that indicates whether a type is higher in a hierarchy than the type.

func isSupertype(of: UTType) -> Bool

Returns a Boolean value that indicates whether a type is lower in a hierarchy than the type.

