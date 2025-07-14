

- Core Foundation
-  CFPreferencesSetAppValue(\_:\_:\_:) 

Function

# CFPreferencesSetAppValue(\_:\_:\_:)

Adds, modifies, or removes a preference.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesSetAppValue(
    _ key: CFString,
    _ value: CFPropertyList?,
    _ applicationID: CFString
)
```

## Parameters 

`key`  

The preference key whose value you wish to set.

`value`  

The value to set for the specified `key` and application. Pass `NULL` to remove the specified key from the application’s preferences.

`applicationID`  

The ID of the application whose preferences you wish to create or modify, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

## Discussion

New preference values are stored in the standard application preference location, `~/Library/Preferences/`. When called with kCFPreferencesCurrentApplication, modifications are performed in the preference domain “Current User, Current Application, Any Host.” If you need to create preferences in some other domain, use the low-level function CFPreferencesSetValue(_:_:_:_:_:).

You must call the CFPreferencesAppSynchronize(_:) function in order for your changes to be saved to permanent storage.

## See Also

### Setting Preference Values

func CFPreferencesSetMultiple(CFDictionary?, CFArray?, CFString, CFString, CFString)

Convenience function that allows you to set and remove multiple preference values.

func CFPreferencesSetValue(CFString, CFPropertyList?, CFString, CFString, CFString)

Adds, modifies, or removes a preference value for the specified domain.

