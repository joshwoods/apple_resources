

- StoreKit
- ExternalPurchaseCustomLink
-  showNotice(type:) 

Type Method

# showNotice(type:)

Displays the system disclosure notice sheet and asks the customer whether to continue.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
static func showNotice(type: ExternalPurchaseCustomLink.NoticeType) async throws -> ExternalPurchaseCustomLink.NoticeResult
```

## Parameters 

`type`  

An ExternalPurchaseCustomLink.NoticeType value that determines the disclosure sheet the system displays.

## Return Value

Returns ExternalPurchaseCustomLink.NoticeResult.continued to indicate the customer chooses to continue, or ExternalPurchaseCustomLink.NoticeResult.cancelled to indicate the customer chooses not to continue to view external purchases. This method throws an error if your app isn’t eligible, at runtime, to use this API.

## Discussion

Use this method if your app configures the SKExternalPurchaseCustomLinkRegions property list key.

Call this method to display the system disclosure sheet before your app continues to offer external purchases. Call this method in response to a deliberate customer action, such as tapping a button.

Select the notice type based on how your app presents the custom link to external purchases if the customer chooses to continue:

- Use ExternalPurchaseCustomLink.NoticeType.browser if the app goes to the background, and presents external purchases in a destination outside of the app, which can be an alternative app marketplace, another app, or a website on a browser.

- Use ExternalPurchaseCustomLink.NoticeType.withinApp if the app displays the destination in a web view.

Continue to offer external purchases if showNotice(type:) returns ExternalPurchaseCustomLink.NoticeResult.continued; otherwise don’t continue.

For example code that calls this method, see ExternalPurchaseCustomLink.

## See Also

### Displaying the disclosure sheet

enum NoticeType

The custom link out style that informs the type of disclosure notice to display.

enum NoticeResult

The result of showing the disclosure notice.

