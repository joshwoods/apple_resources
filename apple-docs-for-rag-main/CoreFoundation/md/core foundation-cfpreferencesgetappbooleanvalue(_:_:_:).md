

- Core Foundation
-  CFPreferencesGetAppBooleanValue(\_:\_:\_:) 

Function

# CFPreferencesGetAppBooleanValue(\_:\_:\_:)

Convenience function that directly obtains a Boolean preference value for the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesGetAppBooleanValue(
    _ key: CFString,
    _ applicationID: CFString,
    _ keyExistsAndHasValidFormat: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`key`  

The preference key whose value to obtain. The key must specify a preference whose value is of type `Boolean`.

`applicationID`  

The identifier of the application whose preferences are searched, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, such as `com.foosoft`.

`keyExistsAndHasValidFormat`  

On return, `true` if the preference value for the specified key was located and found to be of type `Boolean`, otherwise `false`.

## Return Value

The preference data for the specified key and application, or if no value was located, `false`.

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

func CFPreferencesGetAppIntegerValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> CFIndex

Convenience function that directly obtains an integer preference value for the specified key.

