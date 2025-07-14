

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionControllerWillStartJob(\_:) 

Instance Method

# printInteractionControllerWillStartJob(\_:)

Tells the delegate that the print job is about to start.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionControllerWillStartJob(_ printInteractionController: UIPrintInteractionController)
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

## Discussion

You can implement this method to do set-up tasks related to the print job. For example, an application that needs to do intensive rendering could implement this method to pause animations. This method is called before drawing begins but after the printing user interface is dismissed.

## See Also

### Related Documentation

func printInteractionControllerDidDismissPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is dismissing the printing-options user interface.

### Responding to the Start and End of a Print Job

func printInteractionControllerDidFinishJob(UIPrintInteractionController)

Tells the delegate that the print job has ended.

