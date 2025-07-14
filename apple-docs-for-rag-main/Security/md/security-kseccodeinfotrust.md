

- Security
-  kSecCodeInfoTrust 

Global Variable

# kSecCodeInfoTrust

A key whose value is the trust object the system uses to evaluate the validity of the code’s signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoTrust: CFString
```

## Discussion

The value is a retained SecTrust object. You may use SecTrust functions (see Certificate, Key, and Trust Services to extract detailed information, for example the reasons why certificate validation may have failed. Because this object may continue to be used for further evaluations of the code signature, if you make any changes to it, the behavior of the SecTrust functions is undefined.

Specify the kSecCSSigningInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

