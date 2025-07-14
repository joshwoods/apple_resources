

- Core Services
- Launch Services
-  kLSMultipleSessionsNotSupportedErr 

Global Variable

# kLSMultipleSessionsNotSupportedErr

The requested app can’t run simultaneously in two different user sessions.

Mac Catalyst 13.0+macOS 10.3+

``` source
var kLSMultipleSessionsNotSupportedErr: OSStatus { get }
```

## See Also

### Result Codes

var kLSAppInTrashErr: OSStatus

The app can’t run because it’s inside a Trash folder.

var kLSUnknownErr: OSStatus

An unknown error has occurred.

var kLSNotAnApplicationErr: OSStatus

The item for registration is not an app.

var kLSDataUnavailableErr: OSStatus

Data of the desired type is not available (for example, there is no kind string).

var kLSApplicationNotFoundErr: OSStatus

No app in the Launch Services database matches the input criteria.

var kLSDataErr: OSStatus

Improper data structure.

var kLSLaunchInProgressErr: OSStatus

A launch of the app is already in progress.

var kLSServerCommunicationErr: OSStatus

There is a problem communicating with the server process that maintains the Launch Services database.

var kLSCannotSetInfoErr: OSStatus

The system can’t hide the filename extension.

var kLSIncompatibleSystemVersionErr: OSStatus

The requested app can’t run on the current macOS version.

var kLSNoLaunchPermissionErr: OSStatus

The user doesn’t have permission to launch the app on a managed network.

var kLSNoExecutableErr: OSStatus

The executable file is missing or has an unusable format.

