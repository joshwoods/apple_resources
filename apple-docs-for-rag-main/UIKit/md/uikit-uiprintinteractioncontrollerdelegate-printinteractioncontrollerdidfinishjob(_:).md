

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionControllerDidFinishJob(\_:) 

Instance Method

# printInteractionControllerDidFinishJob(\_:)

Tells the delegate that the print job has ended.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionControllerDidFinishJob(_ printInteractionController: UIPrintInteractionController)
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

## Discussion

You can implement this method to do clean-up tasks related to the print job. This method is called after the last page of the print job is generated but before the completion handler (a block handler of type UIPrintInteractionController.CompletionHandler) is called.

## See Also

### Responding to the Start and End of a Print Job

func printInteractionControllerWillStartJob(UIPrintInteractionController)

Tells the delegate that the print job is about to start.

