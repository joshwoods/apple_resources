

- UIKit
- UIActivity
- UIActivity.ActivityType
-  sharePlay 

Type Property

# sharePlay

A type of activity that makes the provided content available through SharePlay.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
static let sharePlay: UIActivity.ActivityType
```

## Discussion

When using this service, you can use registerGroupActivity(_:) to provide an NSItemProvider with a GroupActivity object as an activity item. If no `GroupActivity` object is provided, the service will start a FaceTime call without an accompanying SharePlay session.

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

