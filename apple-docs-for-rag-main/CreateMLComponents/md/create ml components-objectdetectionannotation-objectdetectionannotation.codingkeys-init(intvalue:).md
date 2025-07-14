

- Create ML Components
- ObjectDetectionAnnotation
- ObjectDetectionAnnotation.CodingKeys
-  init(intValue:) 

Initializer

# init(intValue:)

Creates a new instance from the specified integer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init?(intValue: Int)
```

## Parameters 

`intValue`  

The integer value of the desired key.

## Discussion

If the value passed as `intValue` does not correspond to any instance of this type, the result is `nil`.

## See Also

### Creating a key

init?(rawValue: String)

Creates a new instance with the specified raw value.

init?(stringValue: String)

Creates a new instance from the given string.

