

- Core Foundation
-  CFPreferencesSynchronize(\_:\_:\_:) 

Function

# CFPreferencesSynchronize(\_:\_:\_:)

For the specified domain, writes all pending changes to preference data to permanent storage, and reads latest preference data from permanent storage.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesSynchronize(
    _ applicationID: CFString,
    _ userName: CFString,
    _ hostName: CFString
) -> Bool
```

## Parameters 

`applicationID`  

The ID of the application whose preferences you wish to modify. Takes the form of a Java package name, `com.foosoft`.

`userName`  

kCFPreferencesCurrentUser to modify the current user’s preferences, otherwise kCFPreferencesAnyUser to modify the preferences of all users.

`hostName`  

kCFPreferencesCurrentHost to search the current-host domain, otherwise kCFPreferencesAnyHost to search the any-host domain.

## Return Value

`true` if synchronization was successful, `false` if an error occurred.

## Discussion

This function is the primitive synchronize mechanism for the higher level preference function CFPreferencesAppSynchronize(_:); it writes updated preferences to permanent storage, and reads the latest preferences from permanent storage. Only the exact domain specified is modified. Note that to modify “Any User” preferences requires root privileges (or Admin privileges prior to OS X v10.6)—see Authorization Services Programming Guide.

Do not use this function directly unless you have a specific need. All arguments must be non- `NULL`. Do not use arbitrary user and host names, instead pass the pre-defined constants.

## See Also

### Synchronizing Preferences

func CFPreferencesAppSynchronize(CFString) -> Bool

Writes to permanent storage all pending changes to the preference data for the application, and reads the latest preference data from permanent storage.

