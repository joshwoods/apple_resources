

- ManagedAppDistribution
- ManagedContentView
-  init(primaryLabel:secondaryLabel:tertiaryLabel:quaternaryLabel:offerState:offerAction:icon:) 

Initializer

# init(primaryLabel:secondaryLabel:tertiaryLabel:quaternaryLabel:offerState:offerAction:icon:)

Create a view with the layout of a managed app view and customized labels using localized string keys.

ManagedAppDistributionSwiftUIiOS 17.2+iPadOS 17.2+

``` source
nonisolated
init(
    primaryLabel: LocalizedStringKey,
    secondaryLabel: LocalizedStringKey = "",
    tertiaryLabel: LocalizedStringKey = "",
    quaternaryLabel: LocalizedStringKey = "",
    offerState: ManagedContentOfferState,
    offerAction: @escaping (ManagedContentOfferState) -> Void,
    @ViewBuilder icon: () -> Icon
)
```

## Parameters 

`primaryLabel`  

The localized string key for the primary label.

`secondaryLabel`  

The localized string key for the secondary label.

`tertiaryLabel`  

The localized string key for the tertiary label.

`quaternaryLabel`  

The localized string key for the quaternary label.

`offerState`  

The view’s offer state.

`offerAction`  

The action to execute when a person taps the offer button.

`icon`  

A view that represents the icon for this managed content.

## See Also

### Creating views

init(primaryLabel: any StringProtocol, secondaryLabel: any StringProtocol, tertiaryLabel: any StringProtocol, quaternaryLabel: any StringProtocol, offerState: ManagedContentOfferState, offerAction: (ManagedContentOfferState) -> Void, icon: () -> Icon)

Create a content view with the layout of a managed app view and customized labels using strings.

