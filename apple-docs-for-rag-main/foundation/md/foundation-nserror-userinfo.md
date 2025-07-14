

- Foundation
- NSError
-  userInfo 

Instance Property

# userInfo

The user info dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: [String : Any] { get }
```

## Discussion

If the user info dictionary has not been set, this property is `nil`.

On macOS 10.8 or later, if the user info dictionary has not been set, this property returns an empty dictionary.

## See Also

### Related Documentation

var localizedDescription: String

A string containing the localized description of the error.

### Getting Error Properties

var code: Int

The error code.

var domain: String

A string containing the error domain.

