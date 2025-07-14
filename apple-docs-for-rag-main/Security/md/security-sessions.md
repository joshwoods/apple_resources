

- Security
-  Sessions 

API Collection

# Sessions

Manage login, authorization, and security sessions in macOS.

## Overview

Use the `Security.AuthSession` API to work with session management and inquiry functions.

## Topics

### Creating a Session

func SessionCreate(SessionCreationFlags, SessionAttributeBits) -> OSStatus

Creates a security session.

struct SessionCreationFlags

The flags that affect the creation of a security session.

struct SessionAttributeBits

The attributes of a security session.

### Session Information

func SessionGetInfo(SecuritySessionId, UnsafeMutablePointer&lt;SecuritySessionId>?, UnsafeMutablePointer&lt;SessionAttributeBits>?) -> OSStatus

Obtains information about a security session.

Session ID Values

Use these values as placeholders for specific sessions.

typealias SecuritySessionId

A type that contains an authorization session identifier.

### Result Codes

Sessions API Result Codes

Recognize result codes specific to the sessions API.

