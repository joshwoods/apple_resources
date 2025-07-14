

- Security
-  SecCodeStatus 

Structure

# SecCodeStatus

Operational flags attached by code signing services to running code.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecCodeStatus
```

## Overview

These flags are maintained by the code’s host, and can be read by anyone. Running code may change its own flags, and root may change anyone’s flags. However, each of these flags can change in only one direction and never back, for the lifetime of the code. Not even root can violate this restriction.

All of the bits in the SecCodeStatus enumeration are reserved by Apple. If you set any bits not defined here, the behavior is undefined.

## Topics

### Initializers

init(rawValue: UInt32)

### Constants

static var valid: SecCodeStatus

The code is dynamically valid.

static var hard: SecCodeStatus

The code prefers to be denied access to resources if gaining access would invalidate it.

static var kill: SecCodeStatus

The code wants to be terminated if it ever loses its validity.

static var debugged: SecCodeStatus

The code has been debugged by another process that was allowed to do so.

static var platform: SecCodeStatus

The code ships with the operating system and is signed by Apple.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

