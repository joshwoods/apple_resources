

- Matter
- MTRAttributeValueWaiter
-  cancel() 

Instance Method

# cancel()

Cancel the wait for the set of attribute path/value pairs represented by this MTRAttributeValueWaiter. If the completion has not been called yet, it will becalled with MTRErrorCodeCancelled.

iOS 18.3+iPadOS 18.3+Mac Catalyst 18.3+macOS 15.3+tvOS 18.3+visionOS 2.3+watchOS 11.3+

``` source
func cancel()
```

