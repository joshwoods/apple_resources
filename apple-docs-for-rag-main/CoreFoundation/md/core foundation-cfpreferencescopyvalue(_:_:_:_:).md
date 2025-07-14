

- Core Foundation
-  CFPreferencesCopyValue(\_:\_:\_:\_:) 

Function

# CFPreferencesCopyValue(\_:\_:\_:\_:)

Returns a preference value for a given domain.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesCopyValue(
    _ key: CFString,
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
) -> CFPropertyList?
```

## Parameters 

`key`  

Preferences key for the value to obtain.

`applicationID`  

The ID of the application whose preferences are searched. Takes the form of a Java package name, such as `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser if to search the current-user domain, otherwise kCFPreferencesAnyUser to search the any-user domain.

`hostName`  

kCFPreferencesCurrentHost if to search the current-host domain, otherwise kCFPreferencesAnyHost to search the any-host domain.

## Return Value

The preference data for the specified domain. If the no value was located, returns `NULL`. Ownership follows the The Create Rule.

## Discussion

This function is the primitive get mechanism for the higher level preference function CFPreferencesCopyAppValue(_:_:) Unlike the high-level function, CFPreferencesCopyValue(_:_:_:_:) searches only the exact domain specified. Do not use this function directly unless you have a need. All arguments must be non-`NULL`. Do not use arbitrary user and host names, instead pass the pre-defined domain qualifier constants.

Note that values returned from this function are immutable, even if you have recently set the value using a mutable object.

## See Also

### Getting Preference Values

func CFPreferencesCopyAppValue(CFString, CFString) -> CFPropertyList?

Obtains a preference value for the specified key and application.

func CFPreferencesCopyKeyList(CFString, CFString, CFString) -> CFArray?

Constructs and returns the list of all keys set in the specified domain.

func CFPreferencesCopyMultiple(CFArray?, CFString, CFString, CFString) -> CFDictionary

Returns a dictionary containing preference values for multiple keys.

func CFPreferencesGetAppBooleanValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> Bool

Convenience function that directly obtains a Boolean preference value for the specified key.

func CFPreferencesGetAppIntegerValue(CFString, CFString, UnsafeMutablePointer&lt;DarwinBoolean>?) -> CFIndex

Convenience function that directly obtains an integer preference value for the specified key.

