

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Signature
-  signatureData 

Instance Property

# signatureData

The result of signing the data provided by the caller using the requested digital identity.

iOS 18.0+iPadOS 18.0+

``` source
let signatureData: Data
```

## Discussion

The pass determines the signature data format.

## See Also

### Defining the certificate and signed data

let certificate: JPKIPassContents.Certificate&lt;IdentityType>

The certificate associated with an identity document.

