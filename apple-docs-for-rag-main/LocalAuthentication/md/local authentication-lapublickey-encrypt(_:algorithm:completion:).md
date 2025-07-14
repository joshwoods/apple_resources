

- Local Authentication
- LAPublicKey
-  encrypt(\_:algorithm:completion:) 

Instance Method

# encrypt(\_:algorithm:completion:)

Encrypts the data you supply with a given algorithm.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func encrypt(
    _ data: Data,
    algorithm: SecKeyAlgorithm,
    completion handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func encrypt(
    _ data: Data,
    algorithm: SecKeyAlgorithm
) async throws -> Data
```

## Parameters 

`data`  

The data to encrypt.

`algorithm`  

The algorithm to use to encrypt the data.

`handler`  

A completion handler to call when the encryption operation completes.

`data`  
The encrypted data.

`error`  
An error object that indicates why the encryption failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func encrypt(_ data: Data, algorithm: SecKeyAlgorithm) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing cryptographic operations

func exportBytes(completion: (Data?, (any Error)?) -> Void)

Exports the data that represents a public key.

func verify(Data, signature: Data, algorithm: SecKeyAlgorithm, completion: ((any Error)?) -> Void)

Verifies a digital signature for the data you supply.

