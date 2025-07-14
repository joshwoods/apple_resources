

- StoreKit
- AppTransaction
-  preorderDate 

Instance Property

# preorderDate

The date the customer placed an order for the app before it’s available in the App Store.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let preorderDate: Date?
```

## Discussion

This date is present if your app is available for preorder and the customer places an order before your app is available in the App Store. When your app becomes available, the App Store fulfills the customer’s order. The preorderDate remains the same.

Use this date to recognize customers who place preorders.

For more infomation about preorders, see Offering Your Apps for Pre-Order.

## See Also

### Getting purchase dates

let originalPurchaseDate: Date

The date the customer originally purchased the app from the App Store.

