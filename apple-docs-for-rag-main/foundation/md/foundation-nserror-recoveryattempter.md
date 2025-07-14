

- Foundation
- NSError
-  recoveryAttempter 

Instance Property

# recoveryAttempter

The object in the user info dictionary corresponding to the NSRecoveryAttempterErrorKey key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var recoveryAttempter: Any? { get }
```

## Discussion

The recovery attempter must be an instance of a class that conforms to the NSSecureCoding and NSErrorRecoveryAttempting protocols. It must also be able to correctly interpret an index in the localizedRecoveryOptions property.

If userInfo doesn’t contain a value for NSRecoveryAttempterErrorKey, this property is `nil`.

## See Also

### Related Documentation

var localizedRecoveryOptions: [String]?

An array containing the localized titles of buttons appropriate for displaying in an alert panel.

### Getting the Error Recovery Attempter

NSErrorRecoveryAttempting

A set of methods that provide options to recover from an error.

