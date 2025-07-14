

- Uniform Type Identifiers
- UTType
-  isSupertype(of:) 

Instance Method

# isSupertype(of:)

Returns a Boolean value that indicates whether a type is lower in a hierarchy than the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func isSupertype(of type: UTType) -> Bool
```

## Parameters 

`type`  

A UTType instance.

## Return Value

true if `type` directly or indirectly conforms to the type, but returns false if it’s equal to the type.

## See Also

### Checking a type’s relationship to another type

var supertypes: Set&lt;UTType>

The set of types the type directly or indirectly conforms to.

func conforms(to: UTType) -> Bool

Returns a Boolean value that indicates whether a type conforms to the type.

func isSubtype(of: UTType) -> Bool

Returns a Boolean value that indicates whether a type is higher in a hierarchy than the type.

Navigating Hierarchical Data Using Outline and Split Views

Build a structured user interface that simplifies navigation in your app.

