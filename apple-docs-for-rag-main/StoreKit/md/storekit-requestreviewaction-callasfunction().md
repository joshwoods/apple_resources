

- StoreKit
- RequestReviewAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Tells StoreKit to ask the user to rate or review your app, if appropriate.

StoreKitSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
func callAsFunction()
```

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the RequestReviewAction instance that you get from the requestReview environment value.

For information about how Swift uses the callAsFunction()method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

