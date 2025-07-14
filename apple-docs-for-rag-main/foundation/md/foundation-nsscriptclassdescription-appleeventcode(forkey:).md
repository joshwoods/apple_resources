

- Foundation
- NSScriptClassDescription
-  appleEventCode(forKey:) 

Instance Method

# appleEventCode(forKey:)

Returns the Apple event code for the specified attribute or relationship in the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func appleEventCode(forKey key: String) -> FourCharCode
```

## Parameters 

`key`  

The identifying key for an attribute or relationship of the receiver.

## Return Value

The four-character Apple event code associated with the attribute or relationship identified by `key` in the receiver or, if none exists, in the class description for the receiver’s superclass. Returns `0` if no such attribute or relationship is found.

## See Also

### Getting and comparing Apple event codes

var appleEventCode: FourCharCode

Returns the Apple event code associated with the receiver’s class.

func matchesAppleEventCode(FourCharCode) -> Bool

Returns a Boolean value indicating whether a primary or secondary Apple event code in the receiver matches the passed code.

