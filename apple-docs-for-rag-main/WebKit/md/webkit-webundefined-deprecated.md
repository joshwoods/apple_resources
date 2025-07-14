

- WebKit
-  WebUndefined Deprecated

Class

# WebUndefined

`WebUndefined` objects are simply used to represent the JavaScript “undefined” value in methods when bridging between JavaScript and Objective-C. For example, if you invoke a JavaScript function that returns the JavaScript “undefined” value, then a `WebUndefined` object is returned to the Objective-C calling context.

macOS 10.4–10.14Deprecated

``` source
class WebUndefined
```

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Incorporating Scripts (Legacy)

class WebScriptObject

A `WebScriptObject` object is an Objective-C wrapper for a scripting object passed to your application from the scripting environment.

Deprecated

WebScripting

\`WebScripting\` is an informal protocol that defines methods that classes can implement to export their interfaces to a WebScript environment such as JavaScript.

