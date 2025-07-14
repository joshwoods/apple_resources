

- Security
- Code Signing Services
-  Code Signing Information Flags 

API Collection

# Code Signing Information Flags

Use these supplemental flags to retrieve signing information.

## Overview

Use these constants with the SecCodeCopySigningInformation(_:_:_:) function to specify what type of information to return. See Signing Information Dictionary Keys for more information about the information returned.

## Topics

### Constants

var kSecCSInternalInformation: UInt32

Internal code signing information.

var kSecCSSigningInformation: UInt32

Cryptographic signing information.

var kSecCSRequirementInformation: UInt32

Code requirements—including the designated requirement—embedded in the code.

var kSecCSDynamicInformation: UInt32

Dynamic validity information about running code.

var kSecCSContentInformation: UInt32

More information about the file system contents making up the signed code on disk.

var kSecCSSkipResourceDirectory: UInt32

Suppress validating the resource directory.

var kSecCSCalculateCMSDigest: UInt32

