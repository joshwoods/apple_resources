

- Message UI
- MFMessageComposeViewControllerDelegate
-  messageComposeViewController(\_:didFinishWith:) 

Instance Method

# messageComposeViewController(\_:didFinishWith:)

Tells the delegate that the user finished composing the message.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func messageComposeViewController(
    _ controller: MFMessageComposeViewController,
    didFinishWith result: MessageComposeResult
)
```

**Required**

## Parameters 

`controller`  

The message composition view controller that is returning the result.

`result`  

A result code that indicates how the user chose to complete the composition. See the MessageComposeResult enumeration.

## Discussion

This method is called when the user taps one of the buttons to dismiss the message composition interface. Your implementation of this method should dismiss the view controller and perform any additional actions needed to process the sending of the message. The result parameter lets you know whether the user chose to cancel or send the message, or whether sending the message failed.

Implementation of this method is required.

## See Also

### Responding to the Message Completion

enum MessageComposeResult

These constants describe the result of the message-composition interface.

