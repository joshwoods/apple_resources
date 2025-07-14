

- Security
- Code Signing Services
-  Guest Attribute Dictionary Keys 

API Collection

# Guest Attribute Dictionary Keys

Specify attributes of guest code.

## Overview

Use these keys in the dictionary you supply as the `attributes` parameter to the SecHostCreateGuest, SecHostSetGuestStatus, and SecCodeCopyGuestWithAttributes(_:_:_:_:) functions.

## Topics

### Constants

let kSecGuestAttributeArchitecture: CFString

A key whose value is a number representing the CPU type under which the guest code is designed to run.

let kSecGuestAttributeAudit: CFString

let kSecGuestAttributeCanonical: CFString

A key whose value is the guest code object for that guest.

let kSecGuestAttributeDynamicCode: CFString

let kSecGuestAttributeDynamicCodeInfoPlist: CFString

let kSecGuestAttributeHash: CFString

A key whose value is a data object containing the SHA-1 hash of the code directory.

let kSecGuestAttributeMachPort: CFString

Not implemented.

let kSecGuestAttributePid: CFString

A key whose value is an integer of type `pid_t` representing a process ID (PID), usually of the kernel’s guest.

let kSecGuestAttributeSubarchitecture: CFString

A key whose value is a number representing the CPU subtype under which the guest code is designed to run.

