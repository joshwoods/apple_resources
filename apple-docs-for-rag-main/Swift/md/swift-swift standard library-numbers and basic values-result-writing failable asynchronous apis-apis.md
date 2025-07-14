

- Swift
- Swift Standard Library
- Numbers and Basic Values
- Result
-  Writing Failable Asynchronous APIs 

Article

# Writing Failable Asynchronous APIs

Vend results as part of an API when you can’t return errors synchronously.

## Overview

When writing a function, method, or other API that might fail, you use the `throws` keyword on the declaration to indicate that the API call can throw an error. However, you can’t use the `throws` keyword to model APIs that return asynchronously. Instead, use the Result enumeration to capture information about whether an asychronous call succeeds or fails, and use the associated values for the Result.success(_:) and Result.failure(_:) cases to carry information about the result of the call.

### Return Result Instances Asynchronously

The following example models an asynchronous source of random numbers. The `fetchRemoteRandomNumber(completion:)` method returns `Void` synchronously, and asynchronously calls a completion handler with a `Result` instance that contains either a random result or information about the failure.

```
let queue = DispatchQueue(label: "com.example.queue")

enum EntropyError: Error {
    case entropyDepleted
}

struct AsyncRandomGenerator {
    static let entropyLimit = 5
    var count = 0

    mutating func fetchRemoteRandomNumber(
        completion: @escaping (Result) -> Void
    ) {
        let result: Result
        if count 

Users of your remote random number generator can decide how to handle both the success and failure cases:

```
var generator = AsyncRandomGenerator()

// Request one more number than the limit to trigger a failure.
(0..

## See Also

### Representing a Result

case success(Success)

A success, storing a `Success` value.

case failure(Failure)

A failure, storing a `Failure` value.

