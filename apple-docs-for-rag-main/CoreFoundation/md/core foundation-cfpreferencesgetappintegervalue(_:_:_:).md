

- Core Foundation
-  CFPreferencesGetAppIntegerValue(\_:\_:\_:) 

Function

# CFPreferencesGetAppIntegerValue(\_:\_:\_:)

Convenience function that directly obtains an integer preference value for the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesGetAppIntegerValue(
    _ key: CFString,
    _ applicationID: CFString,
    _ keyExistsAndHasValidFormat: UnsafeMutablePointer?
) -> CFIndex
```

## Parameters 

`key`  

The preference key whose value you wish to obtain. The key must specify a preference whose value is of type `int`.

`applicationID`  

The identifier of the application whose preferences you wish to search, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

`keyExistsAndHasValidFormat`  

On return, indicates whether the preference value for the specified key was located and found to be of type `int`.

## Return Value

The preference data for the specified key and application. If no value was located, `0` is returned.

## See Also

### Getting Preference Values

func CFPreferencesCopyAppValue(CFString, CFString) -> CFPropertyList?

Obtains a preference value for the specified key and application.

func CFPreferencesCopyKeyList(CFString, CFString, CFString) -> CFArray?

Constructs and returns the list of all keys set in the specified domain.

func CFPreferencesCopyMultiple(CFArray?, CFString, CFString, CFString) -> CFDictionary

Returns a dictionary containing preference values for multiple keys.

func CFPreferencesCopyValue(CFString, CFString, CFString, CFString) -> CFPropertyList?

Returns a preference value for a given domain.

func CFPreferencesGetAppBooleanValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Bool

Convenience function that directly obtains a Boolean preference value for the specified key.

