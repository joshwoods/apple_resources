

- Security
-  AuthorizationItem 

Structure

# AuthorizationItem

A structure containing information about an authorization right or the authorization environment.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AuthorizationItem
```

## Overview

When using an authorization item to contain a right, set the name field to the name of the right—for example, `"com.myOrganization.myProduct.myRight"`, the valueLength and flags fields to `0`, and the value field to `nil`. For more information on naming rights, read Authorization Services Programming Guide

When using an authorization item for the AuthorizationExecuteWithPrivileges function, set the name field to kAuthorizationRightExecute, and the flags field to `0`. Set the value field to the full POSIX pathname of the tool to execute and the valueLength field to the byte length of the value in the value field.

When using an authorization item to contain environment data, set the name field to the name of the environment data—for example, kAuthorizationEnvironmentUsername—and the flags field to `0`. Set the value field, in this case, to the actual user name and the valueLength field to the byte length of the value in the value field.

## Topics

### Initializers

init(name: AuthorizationString, valueLength: Int, value: UnsafeMutableRawPointer?, flags: UInt32)

Creates a new authorization item.

### Instance Properties

var flags: UInt32

Reserved option bits.

var name: AuthorizationString

The required name of the authorization right or environment data.

var value: UnsafeMutableRawPointer?

A pointer to information pertaining to the name field.

var valueLength: Int

The number of bytes in the value field.

## Relationships

### Conforms To

- BitwiseCopyable

