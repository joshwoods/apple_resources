

- Foundation
- NSScriptClassDescription
-  appleEventCode 

Instance Property

# appleEventCode

Returns the Apple event code associated with the receiver’s class.

Mac Catalyst 13.0+macOS 10.0+

``` source
var appleEventCode: FourCharCode { get }
```

## Return Value

The Apple event code associated with the receiver’s class. This is the primary code used to identify the class in Apple events.

## See Also

### Getting and comparing Apple event codes

func appleEventCode(forKey: String) -> FourCharCode

Returns the Apple event code for the specified attribute or relationship in the receiver.

func matchesAppleEventCode(FourCharCode) -> Bool

Returns a Boolean value indicating whether a primary or secondary Apple event code in the receiver matches the passed code.

