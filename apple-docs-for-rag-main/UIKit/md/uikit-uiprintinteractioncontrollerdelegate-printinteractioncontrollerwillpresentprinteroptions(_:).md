

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionControllerWillPresentPrinterOptions(\_:) 

Instance Method

# printInteractionControllerWillPresentPrinterOptions(\_:)

Tells the delegate that the device is about to display the printing-options user interface.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionControllerWillPresentPrinterOptions(_ printInteractionController: UIPrintInteractionController)
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

## See Also

### Responding to the Presentation and Dismissal of the Printing Interface

func printInteractionControllerDidPresentPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device has presented the printing-options user interface.

func printInteractionControllerWillDismissPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is about to dismiss the printing-options user interface.

func printInteractionControllerDidDismissPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is dismissing the printing-options user interface.

