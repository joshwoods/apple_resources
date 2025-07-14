

- Messages
- MSMessagesAppTranscriptPresentation
-  contentSizeThatFits(\_:) 

Instance Method

# contentSizeThatFits(\_:)

The size of your messages view, given the provided maximum size.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func contentSizeThatFits(_ size: CGSize) -> CGSize
```

**Required**

## Parameters 

`size`  

The maximum available size, in points.

## Discussion

The system calls this method only when the Messages app needs to update the view’s size and the view controller is presenting a live view in the transcript or input field (the view controller’s presentationStyle property is set to the MSMessagesAppPresentationStyle.transcript value). Typically, the view’s size needs updating when the live message is added to the transcript, when the transcript’s width changes, or when the locale or dynamic type size changes.

The MSMessagesAppViewController class’s default implementation of the contentSizeThatFits(_:) method simply returns the `size` parameter. Override this method to return an appropriate size for your live message view that fits within the provided size. The returned value must be equal to or smaller than the `size` parameter.

