

- ClassKit
- CLSBinaryItem
-  valueType 

Instance Property

# valueType

The kind of outcome that the binary activity item represents.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var valueType: CLSBinaryValueType { get }
```

## Discussion

Use this property to indicate how the binary result stored in the value property should be presented to a teacher. For example, you might use a binary item to indicate whether a student passed a quiz, in which case you set valueType to CLSBinaryValueType.passFail. If you use another binary item to indicate whether a student used a hint while taking the quiz, set its valueType to CLSBinaryValueType.yesNo. See the CLSBinaryValueType enumeration for the complete list of possible values.

## See Also

### Managing the Value

var value: Bool

The value that the binary activity item takes.

