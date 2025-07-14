

- Core Foundation
- Preferences Utilities
-  Application, Host, and User Keys 

API Collection

# Application, Host, and User Keys

Keys used to specify the common preference domains.

## Overview

Not all combinations of application, host, and user are supported preference domains. Specifically, `kCFPreferencesAnyHost` is not supported in any combination with other options.

## Topics

### Constants

let kCFPreferencesAnyApplication: CFString

Indicates a preference that applies to any application.

let kCFPreferencesAnyHost: CFString

Indicates a preference that applies to any host.

let kCFPreferencesAnyUser: CFString

Indicates a preference that applies to any user.

let kCFPreferencesCurrentApplication: CFString

Indicates a preference that applies only to the current application.

let kCFPreferencesCurrentHost: CFString

Indicates a preference that applies only to the current host.

let kCFPreferencesCurrentUser: CFString

Indicates a preference that applies only to the current user.

