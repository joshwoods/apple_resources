

- Social
-  SLComposeServiceViewController 

Class

# SLComposeServiceViewController

A view controller that you present from your share app extension, allowing the user to compose social media posts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
class SLComposeServiceViewController
```

## Overview

The SLComposeServiceViewController class provides a standard compose view, and you can present it for social sharing extensions on iOS and macOS. By default, the compose view includes items such as an editable text view and an indication of remaining characters, in addition to support for previewing attachments and displaying configuration items, such as an account or privacy picker.

The compose view controller gets items for the content and preview areas from the extensionContext property of the extension’s NSExtensionContext object.

## Topics

### Configuring the Post Details

func configurationItems() -> [Any]!

Returns configuration items to display in the compose view.

class SLComposeSheetConfigurationItem

An object that provides additional configuration details to use when configuring a composition interface.

func reloadConfigurationItems()

Reloads the list of configuration items.

### Managing the Contents of the Post

var contentText: String!

A string that represents the text which the user entered into the compose view’s text view.

var placeholder: String!

A string that’s displayed in the compose view’s text view when the text view is empty.

var textView: UITextView!

The editable text view in the compose view.

### Presenting the View Controller

func pushConfigurationViewController(UIViewController!)

Presents a configuration view controller that lets the user configure the post.

func popConfigurationViewController()

Dismisses the current configuration view controller.

### Responding to Lifecycle Events

func presentationAnimationDidFinish()

Tells the compose view controller that the presentation animation is finished.

func didSelectCancel()

Sent to the compose view after the cancel animation finishes.

func didSelectPost()

Sent to the compose view after the post animation finishes.

### Canceling a Post

func cancel()

Starts the animated dismissal of the compose view.

### Validating Content

var charactersRemaining: NSNumber!

The number of characters remaining in a custom character limit.

func isContentValid() -> Bool

A Boolean value that indicates whether the current content and attachments are valid.

func validateContent()

Performs validation of the current content and updates the state of the Post button, if appropriate.

### Previewing Attachments

func loadPreviewView() -> UIView!

Loads a view that displays a preview of the attachments in the extension context.

### Enabling Text Autocompletion

var autoCompletionViewController: UIViewController!

The view controller that manages an autocompletion view for suggesting common text completions while users type.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTextDelegate
- NSTextViewDelegate
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIScrollViewDelegate
- UIStateRestoring
- UITextViewDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Composition Interfaces

class SLComposeViewController

A view controller that allows the user to compose social media posts.

