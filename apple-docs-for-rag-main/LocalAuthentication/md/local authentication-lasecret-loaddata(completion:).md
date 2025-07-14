

- Local Authentication
- LASecret
-  loadData(completion:) 

Instance Method

# loadData(completion:)

Retrieves data stored in a secret.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func loadData(completion handler: @escaping (Data?, (any Error)?) -> Void)
```

``` source
var rawData: Data { get async throws }
```

## Parameters 

`handler`  

A completion handler that provides the data stored in a secret.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
var rawData: Data { get async throws }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

