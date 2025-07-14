

- Matter
- MTRBaseClusterAccessControl
-  readAttributeACL(with:completion:) 

Instance Method

# readAttributeACL(with:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func readAttributeACL(
    with params: MTRReadParams?,
    completion: @escaping ([Any]?, (any Error)?) -> Void
)
```

``` source
func readAttributeACL(with params: MTRReadParams?) async throws -> [Any]
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributeACL(with params: MTRReadParams?) async throws -> [Any]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

