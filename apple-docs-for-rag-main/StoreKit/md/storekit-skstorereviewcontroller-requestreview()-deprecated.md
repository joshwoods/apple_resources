

- StoreKit
- SKStoreReviewController
-  requestReview() Deprecated

Type Method

# requestReview()

Tells StoreKit to ask the customer to rate or review your app, if appropriate.

iOS 10.3–14.0DeprecatediPadOS 10.3–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.14–15.0Deprecated

``` source
class func requestReview()
```

Deprecated

For iOS, iPadOS, and apps built with Mac Catalyst, use requestReview(in:) instead.

## Discussion

Although you normally call this method when it makes sense in the user experience flow of your app, App Store policy governs the actual display of a rating and review request view. Because this method may not present an alert, it isn’t appropriate to call requestReview() or requestReview(in:) in response to a button tap or other user action.

Note

When you call this method while your app is in development mode, a rating and review request view is always displayed so you can test the user interface and experience. However, this method has no effect when you call it in an app that you distribute using TestFlight.

When you call this method in your shipping app and the system displays a rating and review request view, the system handles the entire process for you. In addition, you can continue to include a persistent link in the settings or configuration screens of your app that links to your App Store product page. To automatically open a page on which users can write a review in the App Store, append the query parameter `action=write-review` to your product URL.

## See Also

### Indicating an appropriate time for a review

class func requestReview(in: UIWindowScene)

Tells StoreKit to ask the customer to rate or review the app, if appropriate, using the specified scene.

Deprecated

