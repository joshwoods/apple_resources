

- Core Foundation
-  CFPreferencesAppSynchronize(\_:) 

Function

# CFPreferencesAppSynchronize(\_:)

Writes to permanent storage all pending changes to the preference data for the application, and reads the latest preference data from permanent storage.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesAppSynchronize(_ applicationID: CFString) -> Bool
```

## Parameters 

`applicationID`  

The ID of the application whose preferences to write to storage, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

## Return Value

`true` if synchronization was successful, otherwise `false`.

## Discussion

Calling the function CFPreferencesSetAppValue(_:_:_:) is not in itself sufficient for storing preferences. The CFPreferencesAppSynchronize(_:) function writes to permanent storage all pending preference changes for the application. Typically you would call this function after multiple calls to CFPreferencesSetAppValue(_:_:_:). Conversely, preference data is cached after it is first read. Changes made externally are not automatically incorporated. The CFPreferencesAppSynchronize(_:) function reads the latest preferences from permanent storage.

## See Also

### Synchronizing Preferences

func CFPreferencesSynchronize(CFString, CFString, CFString) -> Bool

For the specified domain, writes all pending changes to preference data to permanent storage, and reads latest preference data from permanent storage.

