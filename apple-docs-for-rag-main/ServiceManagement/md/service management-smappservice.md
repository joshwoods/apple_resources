

- Service Management
-  SMAppService 

Class

# SMAppService

An object the framework uses to control helper executables that live inside an app’s main bundle.

Mac Catalyst 16.0+macOS 13.0+

``` source
class SMAppService
```

## Overview

In macOS 13 and later, use `SMAppService` to register and control `LoginItems`, `LaunchAgents`, and `LaunchDaemons` as helper executables for your app. When converting code from earlier versions of macOS, use an `SMAppService` object and select one of the following methods depending on the type of service your helper executable provides:

- For `SMAppServices` initialized as `LoginItems`, the register() and unregister() APIs provide a replacement for SMLoginItemSetEnabled(_:_:).

- For `SMAppServices` initialized as `LaunchAgents`, the register() and unregister() methods provide a replacement for installing property lists in `~/Library/LaunchAgents` or `/Library/LaunchAgents`.

- For `SMAppServices` initialized as `LaunchDaemons`, the register() and unregister() methods provide a replacement for installing property lists in `/Library/LaunchDaemons`.

## Topics

### Registering services

func register() throws

Registers the service so it can begin launching subject to user approval.

func unregister() throws

Unregisters the service so the system no longer launches it.

func unregister(completionHandler: ((any Error)?) -> Void)

Unregisters the service so the system no longer launches it and calls a completion handler you provide with the resulting error value.

### Managing apps

class var mainApp: SMAppService

An app service object that corresponds to the main application as a login item.

class func agent(plistName: String) -> Self

Initializes an app service object with a launch agent with the property list name you provide.

class func daemon(plistName: String) -> Self

Initializes an app service object with a launch daemon with the property list name you provide.

class func loginItem(identifier: String) -> Self

Initializes an app service object for a login item corresponding to the bundle with the identifier you provide.

### Interacting with System Settings

class func openSystemSettingsLoginItems()

Opens System Settings to the Login Items control panel.

### Getting the state of the service

var status: SMAppService.Status

A property that describes registration or authorization state of the service.

enum Status

Constants that describe the registration or authorization status of a helper executable.

### Checking authorization for earlier OS version login items

class func statusForLegacyPlist(at: URL) -> SMAppService.Status

Check the authorization status of an earlier OS version login item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Management

func SMJobBless(CFString!, CFString, AuthorizationRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the executable for the given label as a job to `launchd`.

Deprecated

Authorization Constants

Constants that describe the ability to authorize helper executables or modify daemon applications.

Property List Keys

Property list keys that describe the kinds of applications, daemons, and helper executables the framework manages.

