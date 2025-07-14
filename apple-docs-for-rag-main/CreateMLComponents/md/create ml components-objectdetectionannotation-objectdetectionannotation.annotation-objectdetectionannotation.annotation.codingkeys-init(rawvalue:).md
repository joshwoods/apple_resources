

- Create ML Components
- ObjectDetectionAnnotation
- ObjectDetectionAnnotation.Annotation
- ObjectDetectionAnnotation.Annotation.CodingKeys
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new instance with the specified raw value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init?(rawValue: String)
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

### Creating a key

init?(intValue: Int)

Creates a new instance from the specified integer.

init?(stringValue: String)

Creates a new instance from the given string.

