

- WebKit
- WKNavigationType
-  WKNavigationType.formResubmitted 

Case

# WKNavigationType.formResubmitted

A request to resubmit a form.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
case formResubmitted
```

## Discussion

This type of action occurs when the forward or backward navigation causes the web view to resubmit a form. It also occurs when a reload operation causes the resubmission of the form.

## See Also

### Getting the Navigation Types

case linkActivated

A link activation.

case formSubmitted

A request to submit a form.

case backForward

A request for the frame’s next or previous item.

case reload

A request to reload the webpage.

case other

A navigation request that originates for some other reason.

