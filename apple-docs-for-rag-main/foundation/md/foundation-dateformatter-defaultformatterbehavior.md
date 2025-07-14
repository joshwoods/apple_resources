

- Foundation
- DateFormatter
-  defaultFormatterBehavior 

Type Property

# defaultFormatterBehavior

Returns the default formatting behavior for instances of the class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var defaultFormatterBehavior: DateFormatter.Behavior { get set }
```

## Return Value

The default formatting behavior for instances of the class. For possible values, see DateFormatter.Behavior.

## Discussion

For iOS and for macOS applications linked against macOS 10.5 and later, the default is `NSDateFormatterBehavior10_4`.

## See Also

### Managing Behavior Version

var formatterBehavior: DateFormatter.Behavior

The formatter behavior for the receiver.

