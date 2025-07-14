

- UIKit
- UIActivity
-  UIActivity.ActivityType 

Structure

# UIActivity.ActivityType

A structure that describes the types of activities for which the system has built-in support.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct ActivityType
```

## Overview

These constants represent the values that can be stored in the activityType property of system-defined activity objects.

## Topics

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

static let postToVimeo: UIActivity.ActivityType

A type of activity that posts the provided video to the user’s Vimeo account.

static let postToWeibo: UIActivity.ActivityType

A type of activity that posts the provided content to the user’s Weibo feed.

static let print: UIActivity.ActivityType

A type of activity that prints the provided content.

static let saveToCameraRoll: UIActivity.ActivityType

A type of activity that assigns the image or video to the user’s camera roll.

static let sharePlay: UIActivity.ActivityType

A type of activity that makes the provided content available through SharePlay.

### Initializers

init(String)

Creates an activity type.

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the activity information

class var activityCategory: UIActivity.Category

The category of the activity, which may be used to group activities in the UI.

enum Category

An enumeration that defines categories of activities.

var activityType: UIActivity.ActivityType?

The type of service being provided.

var activityTitle: String?

A user-readable string that describes the service.

var activityImage: UIImage?

An image that identifies the service to the user.

