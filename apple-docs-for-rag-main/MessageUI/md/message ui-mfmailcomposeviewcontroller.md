

- Message UI
-  MFMailComposeViewController 

Class

# MFMailComposeViewController

A standard view controller, whose interface lets the user manage, edit, and send email messages.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class MFMailComposeViewController
```

## Overview

Use this view controller to display a standard email interface inside your app. Before presenting the interface, populate the fields with initial values for the subject, email recipients, body text, and attachments of the email. After presenting the interface, the person can edit your initial values before sending the email.

The composition interface doesn’t guarantee the delivery of your email message; it only lets you construct the initial message and present it for user approval. The person may opt to cancel the composition interface which discards the message and its contents. If the person opts to send the message, the message queues in the user’s Mail app outbox. The Mail app is ultimately responsible for sending the message.

Important

You must not modify the view hierarchy presented by this view controller. However, you can customize the appearance of the interface using the UIAppearance protocol.

An alternate way to compose emails is to create and open a URL that uses the `mailto` scheme. URLs of that type go directly to the built-in Mail app, which uses your URL to configure a message. For information about the structure of `mailto` URLs, see Apple URL Scheme Reference.

### Checking the availability of the composition interface

Before presenting the mail compose view controller, always call the canSendMail() method to see if the person configured the current device to send email. If the person’s device isn’t set up for the delivery of email, you can notify the person or disable the email dispatch features in your application. You shouldn’t attempt to use this interface if the canSendMail() method returns false.

- Swift
- Obj-C

```
if !MFMailComposeViewController.canSendMail() {
    print("Mail services are not available")
    return
}
```

```
if (![MFMailComposeViewController canSendMail]) {
   NSLog(@"Mail services are not available.");
   return;
}
```

### Configuring and displaying the composition interface

After verifying that mail services are available, you can create and configure the mail composition view controller and then present it as any other view controller. Use the methods of this class to specify the subject, recipients, and message body of the email, including any attachments you want to send with the message. The sample code below shows how to configure the composition interface and present it modally. Always assign a delegate to the mailComposeDelegate property, because the delegate is responsible for dismissing the composition interface later.

- Swift
- Obj-C

```
let composeVC = MFMailComposeViewController()
composeVC.mailComposeDelegate = self

// Configure the fields of the interface.
composeVC.setToRecipients(["address@example.com"])
composeVC.setSubject("Hello!")
composeVC.setMessageBody("Hello from California!", isHTML: false)
// Present the view controller modally.
self.present(composeVC, animated: true, completion: nil)
```

```
MFMailComposeViewController* composeVC = [[MFMailComposeViewController alloc] init];
composeVC.mailComposeDelegate = self;

// Configure the fields of the interface.
[composeVC setToRecipients:@[@"address@example.com"]];
[composeVC setSubject:@"Hello!"];
[composeVC setMessageBody:@"Hello from California!" isHTML:NO];

// Present the view controller modally.
[self presentViewController:composeVC animated:YES completion:nil];

```

Important

After presenting a mail compose view controller, the system ignores any attempts to modify the email using the methods of this class. The user can still edit the content of the email, but your app can’t. Therefore, always configure the fields of your email *before* presenting the view controller.

The mail compose view controller isn’t dismissed automatically. When the user taps the buttons to send the email or cancel the interface, the mail compose view controller calls the mailComposeController(_:didFinishWith:error:) method of its delegate. Your implementation of that method must dismiss the view controller explicitly, as shown in sample code below. You can also use this method to check the result of the operation.

- Swift
- Obj-C

```
func mailComposeController(controller: MFMailComposeViewController,
                           didFinishWithResult result: MFMailComposeResult, error: NSError?) {
    // Check the result or perform other tasks.

    // Dismiss the mail compose view controller.
    controller.dismiss(animated: true, completion: nil)
}

```

```
- (void)mailComposeController:(MFMailComposeViewController *)controller
          didFinishWithResult:(MFMailComposeResult)result error:(NSError *)error {
   // Check the result or perform other tasks.

   // Dismiss the mail compose view controller.
   [self dismissViewControllerAnimated:YES completion:nil];
}

```

The user can delete a queued message before it’s sent. Although the view controller reports the success or failure of the operation to its delegate, this class doesn’t provide a way for you to verify if the email sent.

For more information on how to present and dismiss view controllers, see View Controller Programming Guide for iOS.

## Topics

### Responding to the view controller dismissal

var mailComposeDelegate: (any MFMailComposeViewControllerDelegate)?

The mail composition view controller’s delegate.

protocol MFMailComposeViewControllerDelegate

An interface for responding to user interactions with a mail compose view controller.

### Determining mail availability

class func canSendMail() -> Bool

Returns a Boolean that indicates whether the current device is able to send email.

### Setting mail fields programmatically

func setSubject(String)

Sets the initial text for the subject line of the email.

func setToRecipients([String]?)

Sets the initial recipients to include in the email’s To field.

func setCcRecipients([String]?)

Sets the initial recipients to include in the email’s Cc field.

func setBccRecipients([String]?)

Sets the initial recipients to include in the email’s Bcc field.

func setMessageBody(String, isHTML: Bool)

Sets the initial body text to include in the email.

func addAttachmentData(Data, mimeType: String, fileName: String)

Adds the specified data as an attachment to the message.

func setPreferredSendingEmailAddress(String)

Sets the preferred email address to use in the From field, if such an address is available.

### Responding to errors

struct MFMailComposeError

Mail composition errors.

let MFMailComposeErrorDomain: String

The domain used for error objects that are associated with the mail composition interface.

enum Code

Error codes for NSError objects that are associated with the mail composition interface.

### Instance Methods

func insertCollaborationItemProvider(NSItemProvider, completionHandler: (Bool) -> Void)

## Relationships

### Inherits From

- UINavigationController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

