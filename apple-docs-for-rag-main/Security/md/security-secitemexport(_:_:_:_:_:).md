

- Security
-  SecItemExport(\_:\_:\_:\_:\_:) 

Function

# SecItemExport(\_:\_:\_:\_:\_:)

Exports one or more certificates, keys, or identities.

macOS 10.7+

``` source
func SecItemExport(
    _ secItemOrArray: CFTypeRef,
    _ outputFormat: SecExternalFormat,
    _ flags: SecItemImportExportFlags,
    _ keyParams: UnsafePointer?,
    _ exportedData: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`secItemOrArray`  

The keychain item or items to export. You can export only the following types of keychain items: SecCertificate, SecKey, and SecIdentity. If you are exporting exactly one item, you can specify a SecKeychainItem object. Otherwise this parameter is a CFArray object containing a number of items of type SecKeychainItem.

`outputFormat`  

The format of the desired external representation for the item. Set this parameter to SecExternalFormat.formatUnknown to use the default for that item type. Possible values for this parameter and default values are enumerated in SecExternalFormat.

`flags`  

A flag field indicating whether the exported item should have PEM armor. PEM armor refers to a way of expressing binary data as an ASCII string so that it can be transferred over text-only channels such as email. Set this flag to pemArmour if you want PEM armoring.

`keyParams`  

A pointer to a structure containing a set of input parameters for the function. If no key items are being exported, these parameters are optional and you can set the `keyParams` parameter to `NULL`. For more information, see SecItemImportExportKeyParameters.

`exportedData`  

On return, the variable referenced by this argument is overwritten with a CFData object containing the external representation of the keychain item or items. You are responsible for releasing this object by calling CFRelease.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function works only with keys, certificates, and identities. An identity is the combination of a certificate and its associated private key. Although public keys are commonly stored in certificates, they can be stored separately in the keychain as well; for example, when you call the SecKeyCreatePair function to create a key pair, both the public and private keys are stored in the keychain. Use the SecKeychainSearchCopyNext function to find a key or certificate. Use the SecIdentitySearchCopyNext function in the Certificate, Key, and Trust API to find an identity.

