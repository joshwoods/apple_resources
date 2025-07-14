

- Create ML Components
- ObjectDetectionAnnotation
- ObjectDetectionAnnotation.CodingKeys
-  init(stringValue:) 

Initializer

# init(stringValue:)

Creates a new instance from the given string.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init?(stringValue: String)
```

## Parameters 

`stringValue`  

The string value of the desired key.

## Discussion

If the string passed as `stringValue` does not correspond to any instance of this type, the result is `nil`.

## See Also

### Creating a key

init?(intValue: Int)

Creates a new instance from the specified integer.

init?(rawValue: String)

Creates a new instance with the specified raw value.

