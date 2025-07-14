

- Service Management
-  Authorization Constants 

API Collection

# Authorization Constants

Constants that describe the ability to authorize helper executables or modify daemon applications.

## Topics

### Constants

var kSMRightBlessPrivilegedHelper: String

The authorization rights key for approving and installing a privileged helper tool.

var kSMRightBlessPrivilegedHelper: String

The authorization rights key for approving and installing a privileged helper tool.

var kSMRightModifySystemDaemons: String

The authorization rights key for modifying system daemons.

var kSMRightModifySystemDaemons: String

The authorization rights key for modifying system daemons.

## See Also

### Management

class SMAppService

An object the framework uses to control helper executables that live inside an app’s main bundle.

func SMJobBless(CFString!, CFString, AuthorizationRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the executable for the given label as a job to `launchd`.

Deprecated

Property List Keys

Property list keys that describe the kinds of applications, daemons, and helper executables the framework manages.

