

- UIKit
- UITraitEnvironment
-  traitCollectionDidChange(\_:) Deprecated

Instance Method

# traitCollectionDidChange(\_:)

Reports changes in the iOS interface environment.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func traitCollectionDidChange(_ previousTraitCollection: UITraitCollection?)
```

**Required**

Deprecated

In Swift, use registerForTraitChanges(_:handler:) or registerForTraitChanges(_:target:action:) instead. In Objective-C, use registerForTraitChanges:withHandler: or registerForTraitChanges:withTarget:action: instead.

## Parameters 

`previousTraitCollection`  

The UITraitCollection object before the interface environment changed.

## Mentioned in 

Checking the availability of 3D Touch

Responding to changing display modes on Apple TV

Scaling Fonts Automatically

## Discussion

The system calls this method when the iOS interface environment changes. Implement this method in view controllers and views, according to your app’s needs, to respond to such changes. For example, you might adjust the layout of the subviews of a view controller when someone rotates from portrait to landscape orientation. The default implementation of this method is empty.

At the beginning of your implementation, call `super` to ensure that interface elements higher in the view hierarchy have an opportunity to adjust their layout first. Use code similar to this:

```
- (void) traitCollectionDidChange: (UITraitCollection *) previousTraitCollection {
    [super traitCollectionDidChange: previousTraitCollection];
    if ((self.traitCollection.verticalSizeClass != previousTraitCollection.verticalSizeClass)
        || (self.traitCollection.horizontalSizeClass != previousTraitCollection.horizontalSizeClass)) {
        // Your custom implementation here.
    }
}
```

