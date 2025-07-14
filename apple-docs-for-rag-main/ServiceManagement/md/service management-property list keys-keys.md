

- Service Management
-  Property List Keys 

API Collection

# Property List Keys

Property list keys that describe the kinds of applications, daemons, and helper executables the framework manages.

## Topics

### Constants

let kSMDomainSystemLaunchd: CFString!

The system-level launch domain.

let kSMDomainUserLaunchd: CFString!

The user-level launch domain.

## See Also

### Management

class SMAppService

An object the framework uses to control helper executables that live inside an app’s main bundle.

func SMJobBless(CFString!, CFString, AuthorizationRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the executable for the given label as a job to `launchd`.

Deprecated

Authorization Constants

Constants that describe the ability to authorize helper executables or modify daemon applications.

