

- Local Authentication
- LAPrivateKey
-  sign(\_:algorithm:completion:) 

Instance Method

# sign(\_:algorithm:completion:)

Generates a digital signature for the data you supply.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func sign(
    _ data: Data,
    algorithm: SecKeyAlgorithm,
    completion handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func sign(
    _ data: Data,
    algorithm: SecKeyAlgorithm
) async throws -> Data
```

## Parameters 

`data`  

The data to sign. The data is usually the digest of applying a cryptographic hash function to some actual data.

`algorithm`  

An algorithm suitable for this data signing operation. For example, `ecdsaSignatureMessageX962SHA256`.

`handler`  

A completion handler to call when the signing operation completes.

data  
The signature of the data you supply.

error  
An error object that indicates why the signing operation failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func sign(_ data: Data, algorithm: SecKeyAlgorithm) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing cryptographic operations

func decrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Decrypts the data you supply with a given algorithm.

func exchangeKeys(publicKey: Data, algorithm: SecKeyAlgorithm, parameters: [AnyHashable : Any], completion: (Data?, (any Error)?) -> Void)

Performs a Diffie-Hellman style key exchange operation.

