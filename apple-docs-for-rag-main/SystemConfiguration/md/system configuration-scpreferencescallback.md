

- System Configuration
-  SCPreferencesCallBack 

Type Alias

# SCPreferencesCallBack

Type of the callback function used when the preferences have been updated or applied.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias SCPreferencesCallBack = (SCPreferences, SCPreferencesNotification, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`prefs`  

The preferences session.

`notificationType`  

The type of notification, such as changes committed or changes applied. See SCPreferencesNotification for information about possible values.

`info`  

A C pointer to a user-specified block of data.

## Topics

### Fields

prefs

The preferences session.

notificationType

The type of notification, such as changes committed or changes applied. See SCPreferencesNotification for information about possible values.

## See Also

### Data Types

class SCPreferences

The handle to an open preferences session for accessing system configuration preferences.

struct SCPreferencesContext

A structure containing user-specified data and callbacks for accessing system configuration preferences.

