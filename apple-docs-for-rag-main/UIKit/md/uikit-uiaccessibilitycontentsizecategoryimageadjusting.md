

- UIKit
-  UIAccessibilityContentSizeCategoryImageAdjusting 

Protocol

# UIAccessibilityContentSizeCategoryImageAdjusting

Methods to determine when to adjust images for different content size categories.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
protocol UIAccessibilityContentSizeCategoryImageAdjusting : NSObjectProtocol
```

## Overview

Objects adopt this protocol when they support scaling image assets to the size required by the accessibility content size categories. Typically, an object sets the adjustsImageSizeForAccessibilityContentSizeCategory property to true only when its image contains vector data that can scale well to the larger sizes required for accessibility.

## Topics

### Preferring accessibility-specific images

var adjustsImageSizeForAccessibilityContentSizeCategory: Bool

A Boolean value that indicates whether the image size increases to support accessibility content size categories.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextAttachment
- UIButton
- UIImageView

## See Also

### Behaviors

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

protocol UIAccessibilityIdentification

Methods that associate a unique identifier with elements in your user interface.

protocol UIAccessibilityReadingContent

Methods to implement for an object that represents content that users read, such as a book or an article.

struct UIAccessibilityTextualContext

Constants that describe a named context that helps identify and classify the type of text inside an element.

