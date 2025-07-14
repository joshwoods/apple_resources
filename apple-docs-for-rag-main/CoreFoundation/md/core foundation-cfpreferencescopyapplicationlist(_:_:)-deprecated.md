

- Core Foundation
-  CFPreferencesCopyApplicationList(\_:\_:) Deprecated

Function

# CFPreferencesCopyApplicationList(\_:\_:)

Constructs and returns the list of all applications that have preferences in the scope of the specified user and host.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFPreferencesCopyApplicationList(
    _ userName: CFString,
    _ hostName: CFString
) -> CFArray?
```

Deprecated

Unsupported API

## Parameters 

`userName`  

kCFPreferencesCurrentUser to search the current-user domain, otherwise kCFPreferencesAnyUser to search the any-user domain.

`hostName`  

kCFPreferencesCurrentHost to search the current-host domain, otherwise kCFPreferencesAnyHost to search the any-host domain.

## Return Value

The list of application IDs. Ownership follows the The Create Rule.

## See Also

### Miscellaneous Functions

func CFPreferencesAppValueIsForced(CFString, CFString) -> Bool

Determines whether or not a given key has been imposed on the user.

