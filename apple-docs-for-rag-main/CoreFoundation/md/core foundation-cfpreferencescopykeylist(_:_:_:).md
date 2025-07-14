

- Core Foundation
-  CFPreferencesCopyKeyList(\_:\_:\_:) 

Function

# CFPreferencesCopyKeyList(\_:\_:\_:)

Constructs and returns the list of all keys set in the specified domain.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesCopyKeyList(
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
) -> CFArray?
```

## Parameters 

`applicationID`  

The ID of the application whose preferences to search. Takes the form of a Java package name, `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser to search the current-user domain, otherwise kCFPreferencesAnyUser to search the any-user domain.

`hostName`  

kCFPreferencesCurrentHost to search the current-host domain, otherwise kCFPreferencesAnyHost to search the any-host domain.

## Return Value

The list of keys. Ownership follows the The Create Rule.

## See Also

### Getting Preference Values

func CFPreferencesCopyAppValue(CFString, CFString) -> CFPropertyList?

Obtains a preference value for the specified key and application.

func CFPreferencesCopyMultiple(CFArray?, CFString, CFString, CFString) -> CFDictionary

Returns a dictionary containing preference values for multiple keys.

func CFPreferencesCopyValue(CFString, CFString, CFString, CFString) -> CFPropertyList?

Returns a preference value for a given domain.

func CFPreferencesGetAppBooleanValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Bool

Convenience function that directly obtains a Boolean preference value for the specified key.

func CFPreferencesGetAppIntegerValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> CFIndex

Convenience function that directly obtains an integer preference value for the specified key.

