

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  init(encryptionScheme:) 

Initializer

# init(encryptionScheme:)

Instantiates a new request configuration with the given encryption scheme.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
init?(encryptionScheme: PKEncryptionScheme)
```

## Parameters 

`encryptionScheme`  

The encryption scheme to be used in this request. For a list of possible values, see PKEncryptionScheme.

## Return Value

A newly instantiated configuration object.

## Discussion

After instantiating a configuration object, you must also set its cardholderName and primaryAccountSuffix properties before using it to create a PKAddPaymentPassViewController instance.

## See Also

### Creating a request configuration

struct PKEncryptionScheme

Encryption schemes.

