

- UIKit
- Windows and screens
-  Getting the user’s attention with alerts and action sheets 

Article

# Getting the user’s attention with alerts and action sheets

Present important information to the user or prompt the user about an important choice.

## Overview

Display an alert or action sheet when your app requires additional information or acknowledgment from the user. Alerts and action sheets interrupt your app’s normal flow to display a message to the user. In the following image, the left image shows an alert and the right image shows an action sheet. The user dismisses an alert or action sheet by selecting one of the listed options.

Important

Because alerts and action sheets are an interruption, use them sparingly and only when absolutely needed. For detailed guidance on when to use them, see Human Interface Guidelines.

To display an alert or action sheet, create a UIAlertController object, configure it, and call its present(_:animated:completion:) method, as shown in the following code. Configuring the alert controller includes specifying the title and message that you want the user to see and the actions the user can select. You must add at least one action — represented by a UIAlertAction object — to an alert controller before presenting it.

```
@IBAction func agreeToTerms() {
   // Create the action buttons for the alert.
   let defaultAction = UIAlertAction(title: "Agree", 
                        style: .default) { (action) in
   // Respond to user selection of the action.
   }
   let cancelAction = UIAlertAction(title: "Disagree", 
                        style: .cancel) { (action) in
   // Respond to user selection of the action.
   }

   // Create and configure the alert controller.     
   let alert = UIAlertController(title: "Terms and Conditions",
         message: "Click Agree to accept the terms and conditions.",
         preferredStyle: .alert)
   alert.addAction(defaultAction)
   alert.addAction(cancelAction)

   self.present(alert, animated: true) {
      // The alert was presented
   }
}
```

### Present an action sheet on iPad

On iPad, UIKit requires that you display an action sheet inside a popover. The following image shows an action sheet anchored to a bar button item.

To display your action sheet in a popover, specify your popover’s anchor point using the popoverPresentationController property of your alert controller. It’s safe to configure this property regardless of the underlying device. In other words, The following code displays the action sheet in a popover on iPad and as a slide-up presentation on iPhone.

```
@IBAction func deleteItem() {
   let destroyAction = UIAlertAction(title: "Delete", 
             style: .destructive) { (action) in
   // Respond to user selection of the action
   }
   let cancelAction = UIAlertAction(title: "Cancel", 
             style: .cancel) { (action) in
   // Respond to user selection of the action
   }

   let alert = UIAlertController(title: "Delete the image?", 
               message: "", 
               preferredStyle: .actionSheet)
   alert.addAction(destroyAction)
   alert.addAction(cancelAction)

   // On iPad, action sheets must be presented from a popover.
   alert.popoverPresentationController?.barButtonItem = 
               self.trashButton

   self.present(alert, animated: true) {
      // The alert was presented
   }
}
```

Note

If your set of actions includes a button configured with the UIAlertAction.Style.cancel style, UIKit removes that button when displaying your action sheet in a popover. Tapping anywhere outside of the popover has the same effect as tapping the Cancel button, including calling your action handler.

## See Also

### Alerts

class UIAlertController

An object that displays an alert message.

class UIAlertAction

An action that can be taken when the user taps a button in an alert.

