

- WatchKit
-  WKImageAnimatable 

Protocol

# WKImageAnimatable

A collection of methods you can use to control the playback of animated images.

watchOS

``` source
protocol WKImageAnimatable : NSObjectProtocol
```

## Overview

Existing classes adopt this protocol and you use the methods to control the animation of those images. Do not adopt this protocol in your own classes.

## Topics

### Animating an Image Sequence

func startAnimating()

Begins animating the current sequence of images.

**Required**

func startAnimatingWithImages(in: NSRange, duration: TimeInterval, repeatCount: Int)

Animates the specified images with the given duration and repeat information.

**Required**

func stopAnimating()

Stops any in-progress animations.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- WKInterfaceGroup
- WKInterfaceImage

## See Also

### Images and movies

class WKInterfaceImage

An image that can be displayed in the interface of your watchOS app.

class WKImage

A wrapper for images you use with a picker interface.

class WKInterfaceMovie

An interface element that lets you play video and audio content in your watchOS app.

class WKInterfaceInlineMovie

An interface element that displays a video’s poster image and supports inline playing of the video.

class WKInterfaceHMCamera

An interface element that displays either a video stream or a single snapshot from an IP camera connected to HomeKit.

enum WKVideoGravity

Constants indicating the appearance of video content.

