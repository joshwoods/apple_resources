

- UIKit
- UIActivity
- UIActivity.ActivityType
-  mail 

Type Property

# mail

A type of activity that posts the provided content to a new email message.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let mail: UIActivity.ActivityType
```

## Discussion

When using this service, you can provide NSString and UIImage objects and NSURL objects pointing to local files as data for the activity items.

To specify an NSData object, you must implement the UIActivityItemSource protocol, return the data object in activityViewController(_:itemForActivityType:), and return the data object’s UTI in activityViewController(_:dataTypeIdentifierForActivityType:). Also, you may need to register the appropriate mapping so that the MIME type can be determined.

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

static let markupAsPDF: UIActivity.ActivityType

A type of activity that marks up the provided content as a PDF file.

static let message: UIActivity.ActivityType

A type of activity that posts the provided content to the Messages app.

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

