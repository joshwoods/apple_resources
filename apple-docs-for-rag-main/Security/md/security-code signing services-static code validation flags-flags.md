

- Security
- Code Signing Services
-  Static Code Validation Flags 

API Collection

# Static Code Validation Flags

Use these supplemental flags to test the validity of a static code signature.

## Overview

These flags supplement the flags described in SecCSFlags. Use these additional constants with the flags parameter of the SecStaticCodeCheckValidity(_:_:_:) and SecStaticCodeCheckValidityWithErrors(_:_:_:_:) functions to control the validation of code in the file system.

## Topics

### Constants

var kSecCSCheckAllArchitectures: UInt32

For multi-architecture (universal) Mach-O programs, validate all architectures included.

var kSecCSDoNotValidateExecutable: UInt32

Do not validate the contents of the main executable.

var kSecCSDoNotValidateResources: UInt32

Do not validate the presence and contents of all bundle resources (if any).

var kSecCSBasicValidateOnly: UInt32

Do not validate either the main executable or the bundle resources, if any.

var kSecCSCheckNestedCode: UInt32

For code in bundle form, locate and recursively check embedded code.

var kSecCSStrictValidate: UInt32

Perform additional checks to ensure the validity of code in bundle form.

var kSecCSFullReport: UInt32

var kSecCSCheckGatekeeperArchitectures: UInt32

var kSecCSRestrictSymlinks: UInt32

var kSecCSRestrictToAppLike: UInt32

var kSecCSRestrictSidebandData: UInt32

var kSecCSUseSoftwareSigningCert: UInt32

var kSecCSValidatePEH: UInt32

var kSecCSSingleThreaded: UInt32

