

- Metal Performance Shaders
- MPSAccelerationStructure
-  rebuild(completionHandler:) Deprecated

Instance Method

# rebuild(completionHandler:)

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.0–17.0DeprecatedmacOS 10.14–14.0DeprecatedtvOS 12.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func rebuild(completionHandler: @escaping MPSAccelerationStructureCompletionHandler)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func rebuild() async -> MPSAccelerationStructure?

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

