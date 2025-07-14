

- StoreKit
- StoreContentBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func buildExpression(_ content: Content) -> some StoreContent where Content : StoreContent
```

## See Also

### Building store content

static func buildBlock&lt;each Content>(repeat each Content) -> TupleStoreContent&lt;repeat each Content>

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

static func buildIf&lt;Content>(Content?) -> Content?

static func buildLimitedAvailability(any StoreContent) -> some StoreContent

struct TupleStoreContent

