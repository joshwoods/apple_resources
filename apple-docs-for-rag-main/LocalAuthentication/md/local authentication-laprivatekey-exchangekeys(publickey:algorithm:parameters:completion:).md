

- Local Authentication
- LAPrivateKey
-  exchangeKeys(publicKey:algorithm:parameters:completion:) 

Instance Method

# exchangeKeys(publicKey:algorithm:parameters:completion:)

Performs a Diffie-Hellman style key exchange operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func exchangeKeys(
    publicKey: Data,
    algorithm: SecKeyAlgorithm,
    parameters: [AnyHashable : Any],
    completion handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func exchangeKeys(
    publicKey: Data,
    algorithm: SecKeyAlgorithm,
    parameters: [AnyHashable : Any]
) async throws -> Data
```

## Parameters 

`publicKey`  

The remote party’s public key.

`algorithm`  

An algorithm suitable for performing this key exchange. For example, `ecdhKeyExchangeCofactorX963SHA256`.

`parameters`  

A dictionary with parameters for this key exchange.

`handler`  

A completion handler to call when the key exchange operation completes.

data  
The result of the key exchange operation.

error  
An error object that indicates why the key exchange failed, or `nil` if the exchange succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func exchangeKeys(publicKey: Data, algorithm: SecKeyAlgorithm, parameters: [AnyHashable : Any]) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The algorithm you use determines the parameters in the dictionary that are required or optional. For more information, see SecKeyKeyExchangeParameter.

## See Also

### Performing cryptographic operations

func decrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Decrypts the data you supply with a given algorithm.

func sign(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Generates a digital signature for the data you supply.

