

- Core Foundation
-  CFPreferencesSetMultiple(\_:\_:\_:\_:\_:) 

Function

# CFPreferencesSetMultiple(\_:\_:\_:\_:\_:)

Convenience function that allows you to set and remove multiple preference values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesSetMultiple(
    _ keysToSet: CFDictionary?,
    _ keysToRemove: CFArray?,
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
)
```

## Parameters 

`keysToSet`  

A dictionary containing the key/value pairs for the preferences to set.

`keysToRemove`  

An array containing a list of keys to remove.

`applicationID`  

The ID of the application whose preferences you wish to modify. Takes the form of a Java package name, `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser to modify the current user’s preferences, otherwise kCFPreferencesAnyUser to modify the preferences of all users.

`hostName`  

kCFPreferencesCurrentHost to modify the preferences of the current host, otherwise kCFPreferencesAnyHost to modify the preferences of all hosts.

## Discussion

Behavior is undefined if a key is in both `keysToSet` and `keysToRemove`

## See Also

### Setting Preference Values

func CFPreferencesSetAppValue(CFString, CFPropertyList?, CFString)

Adds, modifies, or removes a preference.

func CFPreferencesSetValue(CFString, CFPropertyList?, CFString, CFString, CFString)

Adds, modifies, or removes a preference value for the specified domain.

