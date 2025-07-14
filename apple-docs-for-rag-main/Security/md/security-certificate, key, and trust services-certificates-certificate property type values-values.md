

- Security
- Certificate, Key, and Trust Services
- Certificates
-  Certificate Property Type Values 

API Collection

# Certificate Property Type Values

Recognize the possible certificate property types.

## Overview

These are the possible values that may be assigned to the kSecPropertyKeyType key in each of the property dictionaries returned by a call to the SecCertificateCopyValues(_:_:_:) function.

## Topics

### Constants

let kSecPropertyTypeWarning: CFString

A key whose value is a string describing a trust evaluation warning.

let kSecPropertyTypeSuccess: CFString

A key whose value is a string describing a trust evaluation success.

let kSecPropertyTypeSection: CFString

A key whose value is a string describing the name of a field in the certificate (`CFSTR("Subject Name")`, for example).

let kSecPropertyTypeData: CFString

A key whose value is a data object.

let kSecPropertyTypeString: CFString

A key whose value is a string.

let kSecPropertyTypeURL: CFString

Specifies a key whose value is a URL.

let kSecPropertyTypeDate: CFString

Specifies a key whose value is a string containing a date (or a string listing the bytes of an invalid date).

let kSecPropertyTypeArray: CFString

Specifies a key whose value is an array.

let kSecPropertyTypeNumber: CFString

Specifies a key whose value is a number.

let kSecPropertyTypeTitle: CFString

Specifies a key whose value is a string containing the title (display name) of the certificate.

let kSecPropertyTypeError: CFString

Specifies a key whose value is a string containing the reason for a trust evaluation failure.

