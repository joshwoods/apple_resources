

- Security
-  SecTrustedApplicationCopyData(\_:\_:) Deprecated

Function

# SecTrustedApplicationCopyData(\_:\_:)

Retrieves the data of a trusted app instance.

macOS 10.0–10.10Deprecated

``` source
func SecTrustedApplicationCopyData(
    _ appRef: SecTrustedApplication,
    _ data: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`appRef`  

A trusted app from which to retrieve data. Use the SecTrustedApplicationCreateFromPath(_:_:) method to create a trusted app instance.

`data`  

On return, points to an opaque data instance. Call the CFRelease method to release the data when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The trusted app instance created by the SecTrustedApplicationCreateFromPath(_:_:) method includes data that uniquely identifies the app, such as a cryptographic hash of the app. The operating system uses this data to verify that the app is unaltered since the trusted app instance was created. When an app requests access to an item in the keychain for which it is designated as a trusted app, the operating system checks this data before granting access.

Use the SecTrustedApplicationCopyData(_:_:) function to extract this data from the trusted app instance for storage or for transmission over the network. Use the SecTrustedApplicationSetData(_:_:) function to insert that data back into a trusted app instance. Note that this data is opaque: there’s no way to interpret it.

