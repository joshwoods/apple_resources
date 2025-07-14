

- Security
- Certificate, Key, and Trust Services
- Certificates
-  Certificate Property Keys 

API Collection

# Certificate Property Keys

Recognize the dictionary keys that taken together define a certificate property.

## Overview

These are the keys that appear in the property dictionaries that describe a certificate. Each property dictionary includes a key for the property type, a label for the property, a localized label, and the property value itself. Many property dictionaries are in turn collected into a larger dictionary that is returned by a call to the SecCertificateCopyValues(_:_:_:) function.

## Topics

### Constants

let kSecPropertyKeyType: CFString

A key whose value indicates the type of certificate property.

let kSecPropertyKeyLabel: CFString

A key whose value is the label for a certificate property.

let kSecPropertyKeyLocalizedLabel: CFString

A key whose value is the localized label for a certificate property.

let kSecPropertyKeyValue: CFString

A key whose value is the value for a certificate property.

