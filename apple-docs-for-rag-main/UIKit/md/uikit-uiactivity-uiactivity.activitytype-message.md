

- UIKit
- UIActivity
- UIActivity.ActivityType
-  message 

Type Property

# message

A type of activity that posts the provided content to the Messages app.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let message: UIActivity.ActivityType
```

## Discussion

When using this service, you can provide NSString and NSAttributedString objects as data for the activity items. You may also specify NSURL objects whose contents use the `sms` scheme.

If the device has MMS or FaceTime enabled, you can provide UIImage, and NSURL objects as data for the activity items.

To specify an NSData object, you must implement the UIActivityItemSource protocol, return the data object in activityViewController(_:itemForActivityType:), and return the data object’s UTI in activityViewController(_:dataTypeIdentifierForActivityType:).

## See Also

### Constants

static let addToHomeScreen: UIActivity.ActivityType

static let addToReadingList: UIActivity.ActivityType

A type of activity that adds the URL to Safari’s reading list.

static let airDrop: UIActivity.ActivityType

A type of activity that makes the provided content available through AirDrop.

static let assignToContact: UIActivity.ActivityType

A type of activity that assigns the image to a contact.

static let collaborationCopyLink: UIActivity.ActivityType

static let collaborationInviteWithLink: UIActivity.ActivityType

static let copyToPasteboard: UIActivity.ActivityType

A type of activity that posts the provided content to the pasteboard.

static let mail: UIActivity.ActivityType

A type of activity that posts the provided content to a new email message.

static let markupAsPDF: UIActivity.ActivityType

A type of activity that marks up the provided content as a PDF file.

static let openInIBooks: UIActivity.ActivityType

A type of activity that opens the content in iBooks.

static let postToFacebook: UIActivity.ActivityType

A type of activity that posts the provided content to the user’s wall on Facebook.

static let postToFlickr: UIActivity.ActivityType

A type of activity that posts the provided image to the user’s Flickr account.

static let postToTencentWeibo: UIActivity.ActivityType

A type of activity that posts the provided content to the user’s Tencent Weibo feed.

static let postToTwitter: UIActivity.ActivityType

A type of activity that posts the provided content to the user’s Twitter feed.

static let postToVimeo: UIActivity.ActivityType

A type of activity that posts the provided video to the user’s Vimeo account.

