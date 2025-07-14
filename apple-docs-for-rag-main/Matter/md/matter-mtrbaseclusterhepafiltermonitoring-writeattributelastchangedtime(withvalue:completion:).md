

- Matter
- MTRBaseClusterHEPAFilterMonitoring
-  writeAttributeLastChangedTime(withValue:completion:) 

Instance Method

# writeAttributeLastChangedTime(withValue:completion:)

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
func writeAttributeLastChangedTime(
    withValue value: NSNumber?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func writeAttributeLastChangedTime(withValue value: NSNumber?) async throws
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeAttributeLastChangedTime(withValue value: NSNumber?) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

