

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Detail
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init?(rawValue: Int)
```

## Parameters 

`rawValue`  

The raw value to use for the new instance.

## Discussion

If there is no value of the type that corresponds with the specified raw value, this initializer returns `nil`. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

print(PaperSize(rawValue: "Legal"))
// Prints "Optional(PaperSize.Legal)"

print(PaperSize(rawValue: "Tabloid"))
// Prints "nil"
```

## See Also

### Using enumeration raw values

var rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

