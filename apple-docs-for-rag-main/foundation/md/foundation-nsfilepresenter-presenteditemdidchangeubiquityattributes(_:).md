

- Foundation
- NSFilePresenter
-  presentedItemDidChangeUbiquityAttributes(\_:) 

Instance Method

# presentedItemDidChangeUbiquityAttributes(\_:)

Tells your object that the file or file package’s ubiquity attributes have changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
optional func presentedItemDidChangeUbiquityAttributes(_ attributes: Set)
```

## Parameters 

`attributes`  

The set of ubiquity attributes that have changed. For information about valid ubiquity attributes, see the observedPresentedItemUbiquityAttributes property.

## Discussion

To specify the ubiquity attributes that trigger notifications, implement your file provider’s observedPresentedItemUbiquityAttributes property. If you do not implement this property, the system sends notifications when any ubiquity attribute changes.

Note

Changes to the ubiquity attributes don’t typically align with presentedItemDidChange() notifications.

## See Also

### Related Documentation

func item(at: URL, didChangeUbiquityAttributes: Set&lt;URLResourceKey>)

Tells observing file providers that the item’s ubiquity attributes have changed.

### Ubiquity Change Notifications

var observedPresentedItemUbiquityAttributes: Set&lt;URLResourceKey>

A list of ubiquity attributes used to generate and send notifications whenever an attribute in the list changes.

