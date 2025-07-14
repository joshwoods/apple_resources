

- AppKit
-  NSSharingService 

Class

# NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

macOS 10.8+

``` source
class NSSharingService
```

## Overview

An NSSharingService object provides a consistent user experience for sharing items—NSURL objects, NSString objects, NSImage objects, video (through file URLs), of any object that implements the NSPasteboardWriting protocol—in macOS.

For any item or group of items, the NSSharingService displays a sheet with the content to share. A sharing service can create a post on a social network like Twitter or Facebook, send a message by email or iMessage, upload videos to viewing services, or send a file using AirDrop.

You can use NSSharingService objects directly in your app. The following example shows how to create a button that shares content directly to a social media service.

```
- (void)awakeFromNib
{
    NSSharingService * service = [NSSharingService sharingServiceNamed:NSSharingServiceNamePostOnTwitter];
    [myShareOnTwitterButton setTitle:service.title];
    [myShareOnTwitterButton setEnabled:[service canPerformWithItems:nil]];
}

- (IBAction)shareOnTwitter:(id)sender
{
    // Items to share
    NSAttributedString *text = [self.textView attributedString];
    NSImage *image = [self.imageView image];
    NSArray * shareItems = [NSArray arrayWithObjects:text, image, nil];

    NSSharingService *service = [NSSharingService sharingServiceNamed:NSSharingServiceNamePostOnTwitter];
    service.delegate = self;
    [service performWithItems:shareItems];
}
```

## Topics

### Creating a Sharing Service

init?(named: NSSharingService.Name)

Returns a sharing service instance representing the specified service name.

init(title: String, image: NSImage, alternateImage: NSImage?, handler: () -> Void)

Creates a custom sharing service object.

struct Name

Constants that describe the sharing services that macOS supports.

### Managing the Delegate

var delegate: (any NSSharingServiceDelegate)?

Specifies the delegate of the sharing service.

protocol NSSharingServiceDelegate

A set of methods that you use to customize the position and animation of a share sheet, and to be notified whether the item is successfully shared.

### Querying Service Availability

class func sharingServices(forItems: [Any]) -> [NSSharingService]

Returns a list of sharing services which could share all the provided items together.

Deprecated

func canPerform(withItems: [Any]?) -> Bool

Returns whether the service can share all the specified items.

### Getting the Service’s Details

var accountName: String?

The account name used for posting on Twitter or Sina Weibo.

var alternateImage: NSImage?

The alternate image representing the sharing service.

var image: NSImage

The primary image representing the sharing service.

var title: String

The title of the sharing service.

### Configuring the Service

var menuItemTitle: String

The title of the service in the Share menu.

var recipients: [String]?

An array containing the user handles of the desired recipients.

var subject: String?

The subject of the post.

### Sharing Items

func perform(withItems: [Any])

Manually performs the service on the provided items.

### Providing CloudKit Share Options

struct CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

### Getting the Shared Items

var attachmentFileURLs: [URL]?

An array of NSURL objects representing the files that were shared.

var messageBody: String?

The message body as a string.

var permanentLink: URL?

A permanent URL (permalink) that your app can use to access the post.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### App Services

class NSSharingServicePicker

A list of sharing services that the user can choose from.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

class NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

protocol NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

Services Functions

Configure the contents of your app’s Services menu.

