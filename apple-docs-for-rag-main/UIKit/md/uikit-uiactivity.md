

- UIKit
-  UIActivity 

Class

# UIActivity

An abstract class that you subclass to implement app-specific services.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIActivity
```

## Mentioned in 

Adding custom actions and activities

## Overview

You should subclass UIActivity only if you want to provide custom services to people. A service takes data that’s passed to it, does something to that data, and returns the results. For example, a social media service might take whatever text, images, or other content is provided to it and post them to a person’s account. Activity objects are used in conjunction with a UIActivityViewController object, which is responsible for presenting services to people.

The system already provides support for many standard services and makes them available through the UIActivityViewController object. For example, the standard activity view controller supports emailing data, posting items to one of a person’s social media accounts, and several other options. You don’t have to provide custom services for any of the built-in types.

### Subclassing notes

This class must be subclassed before it can be used. The job of an activity object is to act on the data provided to it and to provide some meta information that iOS can display to people. For more complex services, an activity object can also display a custom user interface and use it to gather additional information from people.

#### Methods to override

When subclassing, you must always override the following methods and use them to provide information about your service:

- activityType

- activityTitle

- activityImage

- canPerform(withActivityItems:)

- prepare(withActivityItems:)

- activityCategory

If your canPerform(withActivityItems:) method indicates that your subclass is able to operate on the specified data, the active UIActivityViewController object displays your service to people. When a person selects your service, the activity view controller calls the prepare(withActivityItems:) method followed by only one of these methods:

- activityViewController — Returns a view controller to present to a person. If your service requires additional input from a person, override this method and use it to return the view controller object responsible for presenting your custom UI. (You don’t need to present the view controller yourself.) After your view controller object gathers the needed input, it’s responsible for initiating the task associated with the service.

- perform() — Performs the service without displaying any additional UI. If your service doesn’t need additional input from a person, override this method and perform the task associated with the service.

## Topics

### Getting the activity information

class var activityCategory: UIActivity.Category

The category of the activity, which may be used to group activities in the UI.

enum Category

An enumeration that defines categories of activities.

var activityType: UIActivity.ActivityType?

The type of service being provided.

struct ActivityType

A structure that describes the types of activities for which the system has built-in support.

var activityTitle: String?

A user-readable string that describes the service.

var activityImage: UIImage?

An image that identifies the service to the user.

### Performing the activity

func canPerform(withActivityItems: [Any]) -> Bool

Queries whether the service can act on the specified data items.

func prepare(withActivityItems: [Any])

Prepares your service to act on the specified data.

var activityViewController: UIViewController?

The view controller to present to the user.

func perform()

Performs the service when no custom view controller is provided.

func activityDidFinish(Bool)

Notifies the system that your activity object has completed its work.

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

### Services

class UIActivityViewController

A view controller that you use to offer standard services from your app.

protocol UIActivityItemSource

A set of methods that an activity view controller uses to retrieve the data items to act on.

class UIActivityItemProvider

A proxy for data that passes to an activity view controller.

