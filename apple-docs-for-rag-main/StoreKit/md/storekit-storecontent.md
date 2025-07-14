

- StoreKit
-  StoreContent 

Protocol

# StoreContent

A type that represents the content of a store.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
protocol StoreContent
```

## Topics

### Implementing store content

var body: Self.Body

**Required**

associatedtype Body : StoreContent

**Required**

### Configuring store content

func subscriptionStoreOptionGroupStyle(some SubscriptionOptionGroupStyle) -> some StoreContent

func subscriptionStoreButtonLabel(SubscriptionStoreButtonLabel) -> some StoreContent

func storeButton(Visibility, for: StoreButtonKind...) -> some StoreContent

func subscriptionStoreControlStyle&lt;S>(S, placement: S.Placement) -> some StoreContent

func productDescription(Visibility) -> some StoreContent

### Configuring backgrounds

func subscriptionStoreControlBackground(SubscriptionStoreControlBackground) -> some StoreContent

func subscriptionStoreControlBackground(some ShapeStyle) -> some StoreContent

func subscriptionStorePickerItemBackground(some ShapeStyle) -> some StoreContent

func subscriptionStorePickerItemBackground(some ShapeStyle, in: some Shape) -> some StoreContent

### Supporting types

struct IdentifiedStoreContent

The type of SwiftUI view that StoreKit transforms store content into.

## Relationships

### Conforming Types

- SubscriptionOptionGroup
- SubscriptionOptionGroupSet
- SubscriptionOptionSection
- SubscriptionPeriodGroupSet
- TupleStoreContent

## See Also

### Declaring the structure of a subscription store

struct SubscriptionOptionGroup

A group of subscription options that includes optional views for labels and marketing content.

struct SubscriptionOptionGroupSet

A set of groups of subscription options that include optional views for labels and marketing content.

struct SubscriptionPeriodGroupSet

struct SubscriptionOptionSection

struct StoreContentBuilder

A result builder that creates store content from closures that you provide.

