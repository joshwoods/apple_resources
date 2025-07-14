

- Core Foundation
-  CFPreferencesAppValueIsForced(\_:\_:) 

Function

# CFPreferencesAppValueIsForced(\_:\_:)

Determines whether or not a given key has been imposed on the user.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesAppValueIsForced(
    _ key: CFString,
    _ applicationID: CFString
) -> Bool
```

## Parameters 

`key`  

The key you are querying.

`applicationID`  

The application’s ID, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

## Return Value

`true` if value of the key cannot be changed by the user, otherwise `false`.

## Discussion

In cases where machines and/or users are under some kind of management, you should use this function to determine whether or not to disable UI elements corresponding to those preference keys.

## See Also

### Miscellaneous Functions

func CFPreferencesCopyApplicationList(CFString, CFString) -> CFArray?

Constructs and returns the list of all applications that have preferences in the scope of the specified user and host.

Deprecated

