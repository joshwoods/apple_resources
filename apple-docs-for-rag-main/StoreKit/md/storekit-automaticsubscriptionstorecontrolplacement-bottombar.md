

- StoreKit
- AutomaticSubscriptionStoreControlPlacement
-  bottomBar 

Type Property

# bottomBar

A placement that locates the subscription controls in a bar near the bottom of the main scroll view in a subscription store view.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

``` source
static var bottomBar: AutomaticSubscriptionStoreControlPlacement { get }
```

## Discussion

The bottom bar conditonally applies a special visual treatment when it overlaps the main content of the subscription store view. The content within the bottom bar doesn’t scroll with the rest of the content in the main scroll view.

## See Also

### Getting automatic placements

static var automatic: AutomaticSubscriptionStoreControlPlacement

A context-appropriate placement that the system determines automatically.

static var buttonsInBottomBar: AutomaticSubscriptionStoreControlPlacement

A hybrid placement that positions subscription controls within the main scroll view, and places auxiliary buttons in the bottom bar.

static var scrollView: AutomaticSubscriptionStoreControlPlacement

A placement that locates the subscription controls within the main scroll view of a subscription store view.

static var bottom: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the bottom edge of the view.

static var leading: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the leading edge of the view.

static var trailing: AutomaticSubscriptionStoreControlPlacement

A placement that anchors the subscription controls to the trailing edge of the view.

