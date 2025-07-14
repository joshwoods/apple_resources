

- Message UI
-  MFMessageComposeViewControllerDelegate 

Protocol

# MFMessageComposeViewControllerDelegate

An interface for responding to user interactions with a message compose view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol MFMessageComposeViewControllerDelegate : NSObjectProtocol
```

## Overview

The MFMessageComposeViewControllerDelegate protocol defines a single method that custom objects can implement to respond to updates from a message composition view (an instance of the MFMessageComposeViewController class). Use the method of this protocol to respond to the end of the user composing an SMS message. The method includes information about whether the user chose to send or cancel the message, or whether the attempt to send it failed.

## Topics

### Responding to the Message Completion

func messageComposeViewController(MFMessageComposeViewController, didFinishWith: MessageComposeResult)

Tells the delegate that the user finished composing the message.

**Required**

enum MessageComposeResult

These constants describe the result of the message-composition interface.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to the view controller dismissal

var messageComposeDelegate: (any MFMessageComposeViewControllerDelegate)?

The delegate to which message-related notifications should be sent.

