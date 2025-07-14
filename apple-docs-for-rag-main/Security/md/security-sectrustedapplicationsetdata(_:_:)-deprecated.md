

- Security
-  SecTrustedApplicationSetData(\_:\_:) Deprecated

Function

# SecTrustedApplicationSetData(\_:\_:)

Sets the data of a given trusted app instance.

macOS 10.0–10.10Deprecated

``` source
func SecTrustedApplicationSetData(
    _ appRef: SecTrustedApplication,
    _ data: CFData
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`appRef`  

A trusted application object.

`data`  

A reference to the data to set in the trusted application.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

If you use the SecTrustedApplicationCopyData(_:_:) method to extract the data from a trusted app instance for storage or transmission, you can use the SecTrustedApplicationSetData(_:_:) method to insert that data into a new trusted app. Doing so creates an object that identifies the same app as the original trusted app instance.

