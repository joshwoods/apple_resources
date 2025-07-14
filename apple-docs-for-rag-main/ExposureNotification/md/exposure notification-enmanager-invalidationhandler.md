

- Exposure Notification
- ENManager
-  invalidationHandler 

Instance Property

# invalidationHandler

The handler that the framework invokes when invalidation completes.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var invalidationHandler: (() -> Void)? { get set }
```

## Discussion

The framework invokes this handler only once, and clears the property before invoking it to break retain cycles.

