

- UIKit
- UIActivity
-  UIActivity.Category 

Enumeration

# UIActivity.Category

An enumeration that defines categories of activities.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Category
```

## Overview

Activities have a defined category, and the activity UI may show activities grouped by category.

## Topics

### Constants

case action

Activities whose primary purpose is to take an action on the selected item, like copying an image or saving it to the camera roll.

case share

Activities whose primary purpose is to share the selected item, like sending an image by email.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the activity information

class var activityCategory: UIActivity.Category

The category of the activity, which may be used to group activities in the UI.

var activityType: UIActivity.ActivityType?

The type of service being provided.

struct ActivityType

A structure that describes the types of activities for which the system has built-in support.

var activityTitle: String?

A user-readable string that describes the service.

var activityImage: UIImage?

An image that identifies the service to the user.

