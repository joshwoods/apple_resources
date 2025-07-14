

- Message UI
-  MFMessageComposeViewController 

Class

# MFMessageComposeViewController

A standard view controller whose interface lets the user compose and send SMS or MMS messages.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class MFMessageComposeViewController
```

## Overview

Use an MFMessageComposeViewController object to display the standard message composition interface inside your app. Before presenting the interface, populate the fields with the set of initial recipients and the message you want to send. After presenting the interface, a person can edit your initial values before sending the message.

The composition interface doesn’t guarantee the delivery of your message; it only lets you construct the initial message and present it for a person’s approval. The person may opt to cancel the composition interface which discards the message and its contents. If the person opts to send the message, the Messages app takes on the responsibility of sending the message.

Important

You must not modify the view hierarchy presented by this view controller. However, you can customize the appearance of the interface using the UIAppearance protocol.

An alternate way to compose SMS messages is to create and open a URL that uses the `sms` scheme. URLs of that type go directly to the Messages app, which uses your URL to configure the message. For information about the structure of `sms` URLs, see Apple URL Scheme Reference.

### Checking the availability of the composition interface

Before presenting the message compose view controller, always call the canSendText() method to see if the person configured the current device to send messages. If the user’s device isn’t set up to send or receive messages, you can notify the user or disable the messaging features in your application. You shouldn’t attempt to use this interface if the canSendText() method returns false. If messaging is available, you can also use the canSendAttachments() and canSendSubject() methods to determine if those specific messaging features are available.

- Swift
- Obj-C

```
```

```
if (![MFMessageComposeViewController canSendText]) {
   NSLog(@"Message services are not available.");
}
```

### Configuring and displaying the composition interface

After verifying that message services are available, you can create and configure the message composition view controller and then present it like any other view controller. Use the methods of this class to specify the message’s recipients and the contents of the message. If attachments or a subject line are supported, you can set values for them as well. The sample code below shows how to configure the composition interface and present it modally. Always assign a delegate to the messageComposeDelegate property, because the delegate is responsible for dismissing the composition interface later. The delegate object must conform to the MFMessageComposeViewControllerDelegate protocol.

- Swift
- Obj-C

```
```

```
MFMessageComposeViewController* composeVC = [[MFMessageComposeViewController alloc] init];
composeVC.messageComposeDelegate = self;

// Configure the fields of the interface.
composeVC.recipients = @[@"14085551212"];
composeVC.body = @"Hello from California!";

// Present the view controller modally.
[self present:composeVC animated:YES completion:nil];

```

The message compose view controller isn’t dismissed automatically. When the user taps the buttons to send the message or cancel the interface, the message compose view controller calls the messageComposeViewController(_:didFinishWith:) method of its delegate. Your implementation of that method must dismiss the view controller explicitly, as shown in the sample code below. You can also use this method to check the result of the operation.

- Swift
- Obj-C

```
```

```
- (void)messageComposeViewController:(MFMessageComposeViewController *)controller
                 didFinishWithResult:(MessageComposeResult)result {
   // Check the result or perform other tasks.    // Dismiss the message compose view controller.
   [self dismissViewControllerAnimated:YES completion:nil];}

```

For more information on how to present and dismiss view controllers, see View Controller Programming Guide for iOS.

### Detecting changes to the availability of messaging

Add an observer to the MFMessageComposeViewControllerTextMessageAvailabilityDidChange notification to get notified of changes to the messaging capabilities of the current device. The system delivers that notification to your observer when the status of messaging changes.

## Topics

### Responding to the view controller dismissal

var messageComposeDelegate: (any MFMessageComposeViewControllerDelegate)?

The delegate to which message-related notifications should be sent.

protocol MFMessageComposeViewControllerDelegate

An interface for responding to user interactions with a message compose view controller.

### Determining if message composition is available

class func canSendText() -> Bool

Returns a Boolean value that indicates whether the current device is capable of sending text messages.

class func canSendAttachments() -> Bool

Indicates whether or not messages can include attachments.

class func canSendSubject() -> Bool

Indicates whether or not messages can include subject lines, according to the user’s configuration in Settings.

class func isSupportedAttachmentUTI(String) -> Bool

Indicates whether or not the message can accept a file, with the specified UTI, as an attachment.

### Setting the initial message information

var recipients: [String]?

An array of strings that contains the initial recipients of the message.

var subject: String?

The initial subject of the message.

var body: String?

The initial content of the message.

var message: MSMessage?

A message object from your iMessage app extension.

### Managing attachments

func disableUserAttachments()

Disables the camera/attachment button in the message composition view.

var attachments: [[AnyHashable : Any]]?

Returns an array of dictionaries that describe the properties of an attachment.

func addAttachmentURL(URL, withAlternateFilename: String?) -> Bool

Attaches a specified file to the message.

func addAttachmentData(Data, typeIdentifier: String, filename: String) -> Bool

Attaches arbitrary content to the message.

let MFMessageComposeViewControllerAttachmentURL: String

The URL for the item that is attached to the message.

let MFMessageComposeViewControllerAttachmentAlternateFilename: String

The key for the alternate filename for the file-based item attached to the message.

func insertCollaborationItemProvider(NSItemProvider) -> Bool

### Handling notifications

static let MFMessageComposeViewControllerTextMessageAvailabilityDidChange: NSNotification.Name

Posted when the value returned by the class method has changed.

let MFMessageComposeViewControllerTextMessageAvailabilityKey: String

The value of this key is a number object that contains a Boolean value.

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
- Sendable
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

