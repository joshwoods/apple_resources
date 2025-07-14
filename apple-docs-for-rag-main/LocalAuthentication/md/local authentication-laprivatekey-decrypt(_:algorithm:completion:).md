

- Local Authentication
- LAPrivateKey
-  decrypt(\_:algorithm:completion:) 

Instance Method

# decrypt(\_:algorithm:completion:)

Decrypts the data you supply with a given algorithm.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func decrypt(
    _ data: Data,
    algorithm: SecKeyAlgorithm,
    completion handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func decrypt(
    _ data: Data,
    algorithm: SecKeyAlgorithm
) async throws -> Data
```

## Parameters 

`data`  

The data to decrypt.

`algorithm`  

The algorithm to use to decrypt the data.

`handler`  

A completion handler to call when the decryption operation completes.

`data`  
The decrypted data.

`error`  
An error object that indicates why the decryption failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func decrypt(_ data: Data, algorithm: SecKeyAlgorithm) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing cryptographic operations

func exchangeKeys(publicKey: Data, algorithm: SecKeyAlgorithm, parameters: [AnyHashable : Any], completion: (Data?, (any Error)?) -> Void)

Performs a Diffie-Hellman style key exchange operation.

func sign(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Generates a digital signature for the data you supply.

