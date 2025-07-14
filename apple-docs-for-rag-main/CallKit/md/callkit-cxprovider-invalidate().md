

- CallKit
- CXProvider
-  invalidate() 

Instance Method

# invalidate()

Invalidates the provider and completes all active calls with an error.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func invalidate()
```

## Discussion

After a receiver is invalidated, no additional messages are sent to its delegate.

