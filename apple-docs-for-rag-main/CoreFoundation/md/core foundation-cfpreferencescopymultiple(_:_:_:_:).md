

- Core Foundation
-  CFPreferencesCopyMultiple(\_:\_:\_:\_:) 

Function

# CFPreferencesCopyMultiple(\_:\_:\_:\_:)

Returns a dictionary containing preference values for multiple keys.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesCopyMultiple(
    _ keysToFetch: CFArray?,
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
) -> CFDictionary
```

## Parameters 

`keysToFetch`  

An array of preference keys the values of which to obtain.

`applicationID`  

The ID of the application whose preferences are searched. Takes the form of a Java package name, such as `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser to search the current-user domain, otherwise kCFPreferencesAnyUser to search the any-user domain.

`hostName`  

kCFPreferencesCurrentHost to search the current-host domain, otherwise kCFPreferencesAnyHost to search the any-host domain.

## Return Value

A dictionary containing the preference values for the keys specified by `keysToFetch` for the specified domain. If no values were located, returns an empty dictionary. Ownership follows the The Create Rule.

## Discussion

Note that values returned from this function are immutable, even if you have recently set the value using a mutable object.

## See Also

### Getting Preference Values

func CFPreferencesCopyAppValue(CFString, CFString) -> CFPropertyList?

Obtains a preference value for the specified key and application.

func CFPreferencesCopyKeyList(CFString, CFString, CFString) -> CFArray?

Constructs and returns the list of all keys set in the specified domain.

func CFPreferencesCopyValue(CFString, CFString, CFString, CFString) -> CFPropertyList?

Returns a preference value for a given domain.

func CFPreferencesGetAppBooleanValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Bool

Convenience function that directly obtains a Boolean preference value for the specified key.

func CFPreferencesGetAppIntegerValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> CFIndex

Convenience function that directly obtains an integer preference value for the specified key.

