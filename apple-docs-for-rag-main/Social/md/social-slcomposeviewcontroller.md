

- Social
-  SLComposeViewController 

Class

# SLComposeViewController

A view controller that allows the user to compose social media posts.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
class SLComposeViewController
```

## Overview

Use the isAvailable(forServiceType:) class method to check if a service account, such as Twitter, is set up and reachable before presenting this view to the user.

Set the initial content before presenting the view controller to the user. All the methods that set the content of a post return a Boolean value. They return false if the content doesn’t fit in the post or if the view controller has already been presented to the user. You must set all of the content in the post before presenting the view controller to the user. After presenting the view controller, only the user can edit the post.

You can set a handler—using the completionHandler property—to be notified when the user is done composing a post. Note that completion handlers are not called on any particular thread.

## Topics

### Creating a Social Compose View Controller

init!(forServiceType: String!)

Creates a new social compose view controller.

### Checking the Social Service Type

class func isAvailable(forServiceType: String!) -> Bool

Returns A Boolean value that indicates whether you can send a request for a particular service type.

var serviceType: String!

Specifies the social-networking service.

### Specifying the Contents of the Post

func setInitialText(String!) -> Bool

Sets the initial text to be posted.

func add(UIImage!) -> Bool

Adds an image to the post.

func add(URL!) -> Bool

Adds a URL to the post.

func removeAllImages() -> Bool

Removes all images from the post.

func removeAllURLs() -> Bool

Removes all URLs from the post.

### Processing the Results

var completionHandler: SLComposeViewControllerCompletionHandler!

The handler to call when the user is done composing a post.

typealias SLComposeViewControllerCompletionHandler

Defines a handler to call when the user finishes composing a post.

enum SLComposeViewControllerResult

Possible values for the `result` parameter of the completionHandler property.

## Relationships

### Inherits From

- UIViewController

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

## See Also

### Composition Interfaces

class SLComposeServiceViewController

A view controller that you present from your share app extension, allowing the user to compose social media posts.

