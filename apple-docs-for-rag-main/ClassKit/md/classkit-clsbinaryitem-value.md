

- ClassKit
- CLSBinaryItem
-  value 

Instance Property

# value

The value that the binary activity item takes.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var value: Bool { get set }
```

## Discussion

Interpret this value according to the binary activity item’s valueType. For example, if the value type is set to CLSBinaryValueType.passFail, then false means fail, and true means pass.

## See Also

### Managing the Value

var valueType: CLSBinaryValueType

The kind of outcome that the binary activity item represents.

