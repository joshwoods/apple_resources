

- Foundation
- NSFilePresenter
-  observedPresentedItemUbiquityAttributes 

Instance Property

# observedPresentedItemUbiquityAttributes

A list of ubiquity attributes used to generate and send notifications whenever an attribute in the list changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
optional var observedPresentedItemUbiquityAttributes: Set { get }
```

## Discussion

Valid attributes include the isUbiquitousItemKey attribute and any attribute whose name starts with `ubiquitousItem` or `ubiquitousSharedItem` (or `NSURLUbiquitousItem` or `NSURLUbiquitousSharedItem` in Objective-C).

If the property is not implemented, the system generates notifications for all the ubiquity attributes.

The system checks this property only when the file coordinator’s addFilePresenter(_:) method is called. Make all changes to this property before calling addFilePresenter(_:).

## See Also

### Ubiquity Change Notifications

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

Tells your object that the file or file package’s ubiquity attributes have changed.

