

- StoreKit
- CompactPickerSubscriptionStoreControlStyle
- CompactPickerSubscriptionStoreControlStyle.Placement
-  bottomBar 

Type Property

# bottomBar

A placement that locates the compact picker in a bar near the bottom of the main scroll view in a subscription store view.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

``` source
static var bottomBar: CompactPickerSubscriptionStoreControlStyle.Placement { get }
```

## Discussion

The bottom bar conditonally applies a special visual treatment when it overlaps the main content of the subscription store view. The content within the bottom bar doesn’t scroll with the rest of the content in the main scroll view.

## See Also

### Getting a placement

static var automatic: CompactPickerSubscriptionStoreControlStyle.Placement

static var buttonsInBottomBar: CompactPickerSubscriptionStoreControlStyle.Placement

A hybrid placement that positions subscription controls within the main scroll view, and places auxiliary buttons in the bottom bar.

static var scrollView: CompactPickerSubscriptionStoreControlStyle.Placement

