

- Security
- Code Signing Services
-  Guest Creation Flags 

API Collection

# Guest Creation Flags

Use these supplemental flags to create a guest object.

## Overview

These flags supplement the flags described in SecCSFlags. Use these additional constants with the flags parameter of the SecHostCreateGuest function.

## Topics

### Constants

var kSecCSDedicatedHost: UInt32

Declares dedicated hosting for the given host.

var kSecCSGenerateGuestHash: UInt32

Ask the host to generate the unique binary identifier (kSecCodeInfoUnique) from the copy on disk at the path given.

