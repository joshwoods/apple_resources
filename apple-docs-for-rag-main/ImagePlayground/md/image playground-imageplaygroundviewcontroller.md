

- Image Playground
-  ImagePlaygroundViewController 

Class

# ImagePlaygroundViewController

Displays a standard system interface to generate images from the provided input.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
@MainActor @objc @preconcurrency
class ImagePlaygroundViewController
```

## Overview

Present an ImagePlaygroundViewController to display a standard system interface to generate images from a description you provide. People use the view controller interface to generate images and experiment with the contents before returning an image to your app. You can then incorporate that image into your app’s content.

Create an ImagePlaygroundViewController and configure it with an initial description of the image you want before you present it. Specify a text-based description of the image using the concepts property. If you have a starting image that you want to use to create the new image, specify your image in the sourceImage property.

Present this view controller from your interface and wait for it to deliver results to your custom delegate object. If the person approves the image, the view controller sends that image to your app via this delegate object. The view controller also notifies your delegate if the person cancels the operation.

## Topics

### Creating the view controller

init()

Creates a new image-generation view controller for you to present.

### Processing a generated image

var delegate: (any ImagePlaygroundViewController.Delegate)?

The delegate object that receives the generated image and handles events from the view controller.

protocol Delegate

An interface you use to receive images and handle events related to an image-generation view controller.

### Specifying the configuration of the playground

var selectedGenerationStyle: ImagePlaygroundStyle

Generation style to pre-select upong launching the playground among those in `allowedGenerationStyles`.

var allowedGenerationStyles: [ImagePlaygroundStyle]

A list of allowed generation styles to choose from in the playground.

var personalizationPolicy: ImagePlaygroundPersonalizationPolicy

The policy to apply when determining whether to include people in generated images.

enum ImagePlaygroundPersonalizationPolicy

A policy for enabling or disabling personalization in the system interface.

### Specifying the source content

var concepts: [ImagePlaygroundConcept]

An array of elements that describes the expected contents of the image.

var sourceImage: UIImage?

An image to use as source input for generating the new image.

### Getting the feature availability

class var isAvailable: Bool

A Boolean value that indicates whether image generation is available on the current device.

### Managing the view

func viewDidLoad()

func viewDidDisappear()

func viewWillAppear()

### Instance Properties

var isModalInPresentation: Bool

var modalPresentationStyle: UIModalPresentationStyle

The presentation style for modal view controllers.

var preferredContentSize: CGSize

var supportedInterfaceOrientations: UIInterfaceOrientationMask

### Instance Methods

func viewDidDisappear(Bool)

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
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

