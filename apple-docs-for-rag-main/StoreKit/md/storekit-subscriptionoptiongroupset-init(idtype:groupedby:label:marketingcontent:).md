

- StoreKit
- SubscriptionOptionGroupSet
-  init(idType:groupedBy:label:marketingContent:) 

Initializer

# init(idType:groupedBy:label:marketingContent:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    idType: GroupID.Type = GroupID.self,
    groupedBy transform: @escaping (Product) -> GroupID,
    @ViewBuilder label: @escaping (GroupID) -> Label,
    @ViewBuilder marketingContent: @escaping (GroupID) -> MarketingContent
)
```

## See Also

### Creating subscription option group sets

init(idType: GroupID.Type, groupedBy: (Product) -> GroupID, label: (GroupID) -> Label)

