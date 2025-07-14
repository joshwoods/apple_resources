

- UIKit
- UIPresentationController
-  overrideTraitCollection Deprecated

Instance Property

# overrideTraitCollection

Interface traits for the presented view controller, to use in place of traits from the iOS environment.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@NSCopying @MainActor
var overrideTraitCollection: UITraitCollection? { get set }
```

## Mentioned in 

Choosing a Specific Interface Style for Your iOS App

## Discussion

Use this property to provide an interface trait collection for the presented view controller, overriding one or more values in the iOS trait environment.

Each value you place in the overrideTraitCollection property overrides the corresponding value in the iOS trait environment. For example, the following code snippet shows how to override the display scale for the presented view controller, leaving other traits as they are provided by the system. Place such code, typically, in the implementation file for the presenting view controller:

```
presentedVC.presentationController.overrideTraitCollection = [UITraitCollection traitCollectionWithDisplayScale: 1.5];
[self presentViewController: presentedVC animated: NO completion: nil];
```

The *presenting* view controller is not affected by use of this property.

The default value of the overrideTraitCollection property is `nil`, which results in the full iOS trait environment being used by the presented view controller.

