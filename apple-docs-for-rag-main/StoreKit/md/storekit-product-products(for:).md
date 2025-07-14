

- StoreKit
- Product
-  products(for:) 

Type Method

# products(for:)

Requests product data from the App Store.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func products(for identifiers: Identifiers) async throws -> [Product] where Identifiers : Collection, Identifiers.Element == String
```

## Parameters 

`identifiers`  

A collection of unique in-app purchase product identifiers that you previously configured in App Store Connect. StoreKit ignores any duplicate identifiers in the collection.

## Return Value

An array of products, returned from the App Store.

## Discussion

Use this method to get an instance of Product. Your app must have its product identifiers available to provide them to this function. The following example illustrates requesting two products using hard-coded identifiers.

```
let productIdentifiers = ["com.example.productA", "com.example.productB"]
let appProducts = try await Product.products(for: productIdentifiers)
```

You initially create product identifiers when you configure in-app purchases in App Store Connect; for more information, see Create an in-app purchase. Your app can store or retrieve product identifiers in several ways, such as embedding the identifiers in the app bundle, or fetching them from your server.

If any identifiers are invalid or the App Store can’t find them, the App Store excludes them from the return value. The products(for:) function can throw a StoreKitError for system-related errors.

Tip

Use a single request to fetch a large volume of products.

