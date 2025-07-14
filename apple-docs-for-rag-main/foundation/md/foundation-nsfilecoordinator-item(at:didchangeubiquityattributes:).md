

- Foundation
- NSFileCoordinator
-  item(at:didChangeUbiquityAttributes:) 

Instance Method

# item(at:didChangeUbiquityAttributes:)

Tells observing file providers that the item’s ubiquity attributes have changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func item(
    at url: URL,
    didChangeUbiquityAttributes attributes: Set
)
```

## Discussion

This method triggers the NSFilePresenter protocol’s presentedItemDidChangeUbiquityAttributes(_:) method on any file presenters that are observing the item, even if they are running in different processes.

For information about the types of attributes that can trigger notifications, see the NSFilePresenter protocol’s observedPresentedItemUbiquityAttributes property.

