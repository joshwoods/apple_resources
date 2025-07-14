

- Matter
- MTRBaseClusterGeneralCommissioning
-  readAttributeBasicCommissioningInfo(completion:) 

Instance Method

# readAttributeBasicCommissioningInfo(completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func readAttributeBasicCommissioningInfo(completion: @escaping (MTRGeneralCommissioningClusterBasicCommissioningInfo?, (any Error)?) -> Void)
```

``` source
func readAttributeBasicCommissioningInfo() async throws -> MTRGeneralCommissioningClusterBasicCommissioningInfo
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributeBasicCommissioningInfo() async throws -> MTRGeneralCommissioningClusterBasicCommissioningInfo
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

