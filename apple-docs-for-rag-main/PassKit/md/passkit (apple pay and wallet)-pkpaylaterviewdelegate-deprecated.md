

- PassKit (Apple Pay and Wallet)
-  PKPayLaterViewDelegate Deprecated

Protocol

# PKPayLaterViewDelegate

Methods the framework calls when the Apple Pay Later view’s size changes.

iOS 17.0+iPadOS 17.0+visionOS 1.0+

``` source
protocol PKPayLaterViewDelegate : NSObjectProtocol
```

Deprecated

Apple Pay Later is deprecated.

## Overview

When manually laying out this view, adopt this protocol to receive a callback when the Apple Pay Layer view’s size changes.

## Topics

### Responding to view size changes

func payLaterViewDidUpdateHeight(PKPayLaterView)

Tells the delegate when the Apple Pay Later visual merchandising widget’s height changes.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to changes in the view’s height

var delegate: any PKPayLaterViewDelegate

A delegate object that receives messages about the changes to the Apple Pay Later view.

Deprecated

