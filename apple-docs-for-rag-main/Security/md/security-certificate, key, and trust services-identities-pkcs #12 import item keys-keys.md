

- Security
- Certificate, Key, and Trust Services
- Identities
-  PKCS \#12 Import Item Keys 

API Collection

# PKCS \#12 Import Item Keys

Recognized the dictionary keys returned by an import operation.

## Overview

These keys appear in the dictionary returned by the SecPKCS12Import(_:_:_:) function.

## Topics

### Constants

let kSecImportItemLabel: CFString

Item label.

let kSecImportItemKeyID: CFString

Key ID.

let kSecImportItemTrust: CFString

Trust management object.

let kSecImportItemCertChain: CFString

Certificate list.

let kSecImportItemIdentity: CFString

Identity object.

