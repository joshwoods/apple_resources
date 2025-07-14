

- Image Playground
- ImagePlaygroundViewController
-  ImagePlaygroundViewController.Delegate 

Protocol

# ImagePlaygroundViewController.Delegate

An interface you use to receive images and handle events related to an image-generation view controller.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
@objc(ImageGenerationViewControllerDelegate)
protocol Delegate : NSObjectProtocol
```

## Overview

Adopt the ImagePlaygroundViewController.Delegate protocol in a custom type and assign that type as the delegate of an ImagePlaygroundViewController object. When you present the view controller, the system interface handles interactions with the person and reports the results back to your delegate object.

## Topics

### Receiving the image

func imagePlaygroundViewController(ImagePlaygroundViewController, didCreateImageAt: URL)

Returns the generated image to the delegate.

**Required**

### Handling cancellation events

func imagePlaygroundViewControllerDidCancel(ImagePlaygroundViewController)

Notifies the delegate that the person canceled the generation of the image.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Processing a generated image

var delegate: (any ImagePlaygroundViewController.Delegate)?

The delegate object that receives the generated image and handles events from the view controller.

