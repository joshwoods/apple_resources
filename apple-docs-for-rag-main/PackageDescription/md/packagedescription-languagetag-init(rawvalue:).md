

- PackageDescription
- LanguageTag
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

``` source
init?(rawValue: String)
```

## Parameters 

`rawValue`  

The raw value to use for the new instance.

## Discussion

If there is no value of the type that corresponds with the specified raw value, this initializer returns `nil`.

## See Also

### Creating a Language Tag

init(extendedGraphemeClusterLiteral: String)

Creates an instance initialized to the given value.

init(stringLiteral: String)

Creates an instance initialized to the given value.

init(unicodeScalarLiteral: String)

Creates an instance initialized to the given value.

var rawValue: String

The corresponding value of the raw type.

