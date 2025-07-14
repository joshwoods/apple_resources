

- Local Authentication
- LAPublicKey
-  exportBytes(completion:) 

Instance Method

# exportBytes(completion:)

Exports the data that represents a public key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func exportBytes(completion handler: @escaping (Data?, (any Error)?) -> Void)
```

``` source
var bytes: Data { get async throws }
```

## Parameters 

`handler`  

A completion handler to call when the export operation completes.

`data`  
The data that represents the public key.

`error`  
An error object that indicates why the export operation failed, or `nil` if it succeeded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
var bytes: Data { get async throws }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Performing cryptographic operations

func encrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Encrypts the data you supply with a given algorithm.

func verify(Data, signature: Data, algorithm: SecKeyAlgorithm, completion: ((any Error)?) -> Void)

Verifies a digital signature for the data you supply.

