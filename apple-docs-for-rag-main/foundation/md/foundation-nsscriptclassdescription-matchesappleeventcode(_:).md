

- Foundation
- NSScriptClassDescription
-  matchesAppleEventCode(\_:) 

Instance Method

# matchesAppleEventCode(\_:)

Returns a Boolean value indicating whether a primary or secondary Apple event code in the receiver matches the passed code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func matchesAppleEventCode(_ appleEventCode: FourCharCode) -> Bool
```

## Parameters 

`appleEventCode`  

An Apple event code to compare against the receiver’s primary or secondary codes.

## Return Value

true if the receiver’s primary four-character Apple event code or any of its secondary codes (its synonyms) matches `code`; otherwise, false.

## See Also

### Getting and comparing Apple event codes

var appleEventCode: FourCharCode

Returns the Apple event code associated with the receiver’s class.

func appleEventCode(forKey: String) -> FourCharCode

Returns the Apple event code for the specified attribute or relationship in the receiver.

