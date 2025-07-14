

- Message UI
-  MFMailComposeViewControllerDelegate 

Protocol

# MFMailComposeViewControllerDelegate

An interface for responding to user interactions with a mail compose view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol MFMailComposeViewControllerDelegate : NSObjectProtocol
```

## Overview

The MFMailComposeViewControllerDelegate protocol defines the method that your delegate must implement to manage the mail composition interface. The method of this protocol notifies your delegate object when the user has finished with the interface and is ready to dismiss it.

Your delegate object is responsible for dismissing the picker when the operation completes. You do this by using the dismiss(animated:completion:) method of the parent view controller, which is responsible for displaying the MFMailComposeViewController object’s interface.

## Topics

### Responding to Email Completion

func mailComposeController(MFMailComposeViewController, didFinishWith: MFMailComposeResult, error: (any Error)?)

Tells the delegate that the user wants to dismiss the mail composition view.

**Required**

enum MFMailComposeResult

Result codes returned when the mail composition interface is dismissed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to the view controller dismissal

var mailComposeDelegate: (any MFMailComposeViewControllerDelegate)?

The mail composition view controller’s delegate.

