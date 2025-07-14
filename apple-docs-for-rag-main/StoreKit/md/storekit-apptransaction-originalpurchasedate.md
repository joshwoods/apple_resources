

- StoreKit
- AppTransaction
-  originalPurchaseDate 

Instance Property

# originalPurchaseDate

The date the customer originally purchased the app from the App Store.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let originalPurchaseDate: Date
```

## Discussion

The original purchase date remains the same, even if the customer deletes and reinstalls the app.

In the sandbox testing environment, the original purchase date is always 2013-08-01 12 AM PDT, which is 1375340400000 milliseconds in UNIX epoch time.

## See Also

### Getting purchase dates

let preorderDate: Date?

The date the customer placed an order for the app before it’s available in the App Store.

