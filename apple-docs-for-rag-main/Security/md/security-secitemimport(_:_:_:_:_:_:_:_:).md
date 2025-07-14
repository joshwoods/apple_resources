

- Security
-  SecItemImport(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# SecItemImport(\_:\_:\_:\_:\_:\_:\_:\_:)

Imports one or more certificates, keys, or identities and optionally adds them to a keychain.

macOS 10.7+

``` source
func SecItemImport(
    _ importedData: CFData,
    _ fileNameOrExtension: CFString?,
    _ inputFormat: UnsafeMutablePointer?,
    _ itemType: UnsafeMutablePointer?,
    _ flags: SecItemImportExportFlags,
    _ keyParams: UnsafePointer?,
    _ importKeychain: SecKeychain?,
    _ outItems: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`importedData`  

A CFData object containing the data to import.

`fileNameOrExtension`  

Optional. The name of the file from which the external representation was previously read, or if that is unknown, then the file extension (`.p7r`, for example). This serves as a hint for the key format and key type detection code.

`inputFormat`  

Optional. The address of a SecExternalFormat variable.

If you know what format the external representation is in, set the initial value of this variable to an appropriate format constant to eliminate the need to detect the format. If not, set it to SecExternalFormat.formatUnknown.

On return, the variable referenced by this argument is set to the format that the function actually detected.

Pass `NULL` if you don’t know or don’t care what format the external representation is in.

`itemType`  

Optional. The address of a SecExternalItemType variable.

Before calling this function, if you know what type of key the external representation contains, set the variable to an appropriate type constant to eliminate the need to detect the key type. If not, set it to SecExternalItemType.itemTypeUnknown.

On return, the variable referenced by this argument is set to the type of key that the function actually detected.

Pass `NULL` if you don’t know or don’t care what key type the external representation contains.

`flags`  

A set of import flags. See SecItemImportExportFlags for valid values.

Note that PEM formatting is determined internally via inspection of the incoming data, so the pemArmour flag is ignored.

`keyParams`  

A pointer to a structure containing a set of input parameters for the function. See SecItemImportExportKeyParameters.

`importKeychain`  

Optional. The keychain into which the item should be imported. Pass `NULL` if you do not want to import the item into a keychain.

`outItems`  

Optional. The address of a CFArray variable that, upon return, will contain a list of keychain items. Pass `NULL` if you do not want a copy of these items.

Upon return, the referenced variable is overwritten by a new CFArray array that contains SecKeychainItem objects, each of which may be a SecCertificate, SecKey, or SecIdentity object. The caller is responsible for releasing this CFArray object.

Note

When importing a PKCS12 blob, typically one SecIdentity object and zero or more additional SecCertificate objects are returned in `outItems`. No SecKey objects are returned unless a key is found in the incoming blob that does not have a matching certificate.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function uses the `fileNameOrExtension`, `inputFormat`, and `itemType` parameters to help it interpret the incoming data. In most cases, SecItemImport(_:_:_:_:_:_:_:_:) can correctly interpret an external item if none of these are specified, but it is safer for you not to count on that ability.

When the output item type is SecExternalItemType.itemTypeAggregate, you can use the CFGetTypeID(_:) function to determine the Core Foundation type of each item and the functions in `Getting Information About Keychain Services and Types` to determine the keychain item type of each item. For example, the following code determines whether the item is a certificate:

```
CFTypeID theID = CFGetTypeID(theItem);
if (SecCertificateGetTypeID() == theID)
```

You can pass in `NULL` for both `outItems` and `importKeychain` to determine what is inside a given external data representation. When you do, the function returns the input format and the item type without modifying the data in any way.

