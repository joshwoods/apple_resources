

- Matter
- MTRBaseClusterUnitTesting
-  testSimpleOptionalArgumentRequest(completion:) 

Instance Method

# testSimpleOptionalArgumentRequest(completion:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func testSimpleOptionalArgumentRequest(completion: @escaping MTRStatusCompletion)
```

``` source
func testSimpleOptionalArgumentRequest() async throws
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testSimpleOptionalArgumentRequest() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

