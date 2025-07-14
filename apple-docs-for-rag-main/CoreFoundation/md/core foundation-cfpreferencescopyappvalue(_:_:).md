

- Core Foundation
-  CFPreferencesCopyAppValue(\_:\_:) 

Function

# CFPreferencesCopyAppValue(\_:\_:)

Obtains a preference value for the specified key and application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesCopyAppValue(
    _ key: CFString,
    _ applicationID: CFString
) -> CFPropertyList?
```

## Parameters 

`key`  

The preference key whose value to obtain.

`applicationID`  

The identifier of the application whose preferences to search, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

## Return Value

The preference data for the specified key and application. If no value was located, returns `NULL`. Ownership follows the The Create Rule.

## Discussion

Note that values returned from this function are immutable, even if you have recently set the value using a mutable object.

## See Also

### Getting Preference Values

func CFPreferencesCopyKeyList(CFString, CFString, CFString) -> CFArray?

Constructs and returns the list of all keys set in the specified domain.

func CFPreferencesCopyMultiple(CFArray?, CFString, CFString, CFString) -> CFDictionary

Returns a dictionary containing preference values for multiple keys.

func CFPreferencesCopyValue(CFString, CFString, CFString, CFString) -> CFPropertyList?

Returns a preference value for a given domain.

func CFPreferencesGetAppBooleanValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Bool

Convenience function that directly obtains a Boolean preference value for the specified key.

func CFPreferencesGetAppIntegerValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> CFIndex

Convenience function that directly obtains an integer preference value for the specified key.

