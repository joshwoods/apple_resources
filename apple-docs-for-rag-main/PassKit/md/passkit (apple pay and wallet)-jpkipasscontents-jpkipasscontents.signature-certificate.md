

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Signature
-  certificate 

Instance Property

# certificate

The certificate associated with an identity document.

iOS 18.0+iPadOS 18.0+

``` source
let certificate: JPKIPassContents.Certificate
```

## See Also

### Defining the certificate and signed data

let signatureData: Data

The result of signing the data provided by the caller using the requested digital identity.

