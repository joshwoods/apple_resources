

- UIKit
- UIResponderStandardEditActions
-  printContent(\_:) 

Instance Method

# printContent(\_:)

Tells your app to print available content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
optional func printContent(_ sender: Any?)
```

## Parameters 

`sender`  

The object calling this method.

## Discussion

Implement this method on the responder responsible for printing the contents of the window scene; for instance, the root view controller of a UIWindow. In your implementation, prepare the print job and present an instance of UIPrintInteractionController to show a Print dialog.

- Swift
- Objective-C

```
override func printContent(_ sender: Any?) {
    let info = UIPrintInfo.printInfo()
    info.outputType = .photo
    info.orientation = .portrait
    info.jobName = modelItem.title

    let printInteractionController = UIPrintInteractionController()
    printInteractionController.printInfo = info
    printInteractionController.printingItem = modelItem.image

    let completionHandler: UIPrintInteractionController.CompletionHandler = {
        (controller: UIPrintInteractionController, completed: Bool, error: Error?) in
        if let error = error {
            Logger().error("Print failed due to an error: \(error.localizedDescription)")
        }
    }

    if traitCollection.userInterfaceIdiom == .pad {
        if let printButton = navigationItem.rightBarButtonItem {
            printInteractionController.present(from: printButton, animated: true, completionHandler: completionHandler)
        }
    } else {
        printInteractionController.present(animated: true, completionHandler: completionHandler)
    }
}
```

```
- (void)print:(id)sender {
    UIPrintInfo *info = UIPrintInfo.printInfo;
    info.outputType = UIPrintInfoOutputPhoto;
    info.orientation = UIPrintInfoOrientationPortrait;
    info.jobName = _modelItem.title;

    UIPrintInteractionController *printInteractionController = [[UIPrintInteractionController alloc] init];
    printInteractionController.printInfo = info;
    printInteractionController.printingItem = _modelItem.image;

    UIPrintInteractionCompletionHandler completionHandler = ^(UIPrintInteractionController *printController, BOOL completed, NSError *error) {
        if (error != nil) {
            NSLog(@"Print failed due to an error in domain %@ with error code %lu.", error.domain, (long)error.code);
        }
    };

    if (self.traitCollection.userInterfaceIdiom == UIUserInterfaceIdiomPad) {
        UIBarButtonItem *printButton = self.navigationItem.rightBarButtonItem;
        [printInteractionController presentFromBarButtonItem:printButton animated:YES completionHandler:completionHandler];
    } else {
        [printInteractionController presentAnimated:YES completionHandler: completionHandler];
    }
}
```

If your app includes the UIApplicationSupportsPrintCommand key in its `Info.plist` file, people can print from your app using the keyboard shortcut Command-P, which calls printContent(_:). You can also set printContent(_:) as the action on other print-related controls such as a print button on a toolbar.

For more information about printing from your app, see Printing.

