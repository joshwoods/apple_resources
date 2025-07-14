

- Core Foundation
-  CFPreferencesRemoveSuitePreferencesFromApp(\_:\_:) 

Function

# CFPreferencesRemoveSuitePreferencesFromApp(\_:\_:)

Removes suite preferences from an application’s search chain.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFPreferencesRemoveSuitePreferencesFromApp(
    _ applicationID: CFString,
    _ suiteID: CFString
)
```

## Parameters 

`applicationID`  

The ID of the application from which to remove suite preferences, typically kCFPreferencesCurrentApplication. Do not pass `NULL` or kCFPreferencesAnyApplication. Takes the form of a Java package name, `com.foosoft`.

`suiteID`  

The ID of the application suite preferences to remove. Takes the form of a Java package name, `com.foosoft`.

## See Also

### Adding and Removing Suite Preferences

func CFPreferencesAddSuitePreferencesToApp(CFString, CFString)

Adds suite preferences to an application’s preference search chain.

