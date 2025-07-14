

- TVMLKit
-  TVBrowserViewControllerDelegate 

Protocol

# TVBrowserViewControllerDelegate

Methods for detecting events and performing actions on the browser view.

tvOS 13.0+

``` source
protocol TVBrowserViewControllerDelegate : NSObjectProtocol
```

## Topics

### Managing Focus

func browserViewController(TVBrowserViewController, didCenterOn: TVViewElement)

Tells the delegate how to respond when the specified view element completes the transition to becoming centered upon.

func browserViewController(TVBrowserViewController, willCenterOn: TVViewElement)

Tells the delegate when the specified view element is to be centered on the page.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Interactions with the Browser

var delegate: (any TVBrowserViewControllerDelegate)?

The object that acts as the delegate and handles callbacks for the browser view.

