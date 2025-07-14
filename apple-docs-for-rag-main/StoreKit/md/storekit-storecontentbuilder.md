

- StoreKit
-  StoreContentBuilder 

Structure

# StoreContentBuilder

A result builder that creates store content from closures that you provide.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@resultBuilder
struct StoreContentBuilder
```

## Topics

### Building store content

static func buildBlock&lt;each Content>(repeat each Content) -> TupleStoreContent&lt;repeat each Content>

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

static func buildExpression&lt;Content>(Content) -> some StoreContent

static func buildIf&lt;Content>(Content?) -> Content?

static func buildLimitedAvailability(any StoreContent) -> some StoreContent

struct TupleStoreContent

## See Also

### Declaring the structure of a subscription store

struct SubscriptionOptionGroup

A group of subscription options that includes optional views for labels and marketing content.

struct SubscriptionOptionGroupSet

A set of groups of subscription options that include optional views for labels and marketing content.

struct SubscriptionPeriodGroupSet

struct SubscriptionOptionSection

protocol StoreContent

A type that represents the content of a store.

