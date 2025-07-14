

- Local Authentication
- LAPublicKey
-  verify(\_:signature:algorithm:completion:) 

Instance Method

# verify(\_:signature:algorithm:completion:)

Verifies a digital signature for the data you supply.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func verify(
    _ signedData: Data,
    signature: Data,
    algorithm: SecKeyAlgorithm,
    completion handler: @escaping ((any Error)?) -> Void
)
```

``` source
func verify(
    _ signedData: Data,
    signature: Data,
    algorithm: SecKeyAlgorithm
) async throws
```

## Parameters 

`signedData`  

The signed data.

`signature`  

The signature of the data.

`algorithm`  

An algorithm suitable for verifying signatures with this public key.

`handler`  

A completion handler to call when the verification operation completes.

`error`  
An error object that indicates why the verification operation failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func verify(_ signedData: Data, signature: Data, algorithm: SecKeyAlgorithm) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing cryptographic operations

func encrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Encrypts the data you supply with a given algorithm.

func exportBytes(completion: (Data?, (any Error)?) -> Void)

Exports the data that represents a public key.

