

- Uniform Type Identifiers
- UTType
-  identifier 

Instance Property

# identifier

The string that represents the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var identifier: String { get }
```

## Discussion

The identifier uniquely identifies its type, represented by a reverse-DNS string, such as `public.jpeg` or `com.adobe.pdf`.

API that doesn’t use UTType uses a `String` or CFString to refer to a type by its identifier.

## See Also

### Identifying a type

typealias ReferenceType

An alias for the associated reference type.

