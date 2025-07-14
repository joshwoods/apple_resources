

- Core Foundation
-  CFPreferencesSetValue(\_:\_:\_:\_:\_:) 

Function

# CFPreferencesSetValue(\_:\_:\_:\_:\_:)

Adds, modifies, or removes a preference value for the specified domain.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesSetValue(
    _ key: CFString,
    _ value: CFPropertyList?,
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
)
```

## Parameters 

`key`  

Preferences key for the value you wish to set.

`value`  

The value to set for `key` and application. Pass `NULL` to remove `key` from the domain.

`applicationID`  

The ID of the application whose preferences you wish to modify. Takes the form of a Java package name, `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser to modify the current user’s preferences, otherwise kCFPreferencesAnyUser to modify the preferences of all users.

`hostName`  

kCFPreferencesCurrentHost to modify the preferences of the current host, otherwise kCFPreferencesAnyHost to modify the preferences of all hosts.

## Discussion

This function is the primitive set mechanism for the higher level preference function CFPreferencesSetAppValue(_:_:_:). Only the exact domain specified is modified. Do not use this function directly unless you have a specific need. All arguments except `value` must be non-`NULL`. Do not use arbitrary user and host names, instead pass the pre-defined constants.

You must call the CFPreferencesSynchronize(_:_:_:) function in order for your changes to be saved to permanent storage. Note that you can only save preferences for “Any User” if you have root privileges (or Admin privileges prior to OS X v10.6).

## See Also

### Setting Preference Values

func CFPreferencesSetAppValue(CFString, CFPropertyList?, CFString)

Adds, modifies, or removes a preference.

func CFPreferencesSetMultiple(CFDictionary?, CFArray?, CFString, CFString, CFString)

Convenience function that allows you to set and remove multiple preference values.

