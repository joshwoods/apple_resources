

- UIKit
- UIView
-  draw(\_:for:) 

Instance Method

# draw(\_:for:)

Implemented to draw the view’s content for printing.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
func draw(
    _ rect: CGRect,
    for formatter: UIViewPrintFormatter
)
```

## Parameters 

`rect`  

A rectangle that defines the area for drawing printable content.

`formatter`  

An instance of UIViewPrintFormatter obtained by calling the viewPrintFormatter() method.

## Discussion

You implement this method if you want a view’s printed content to appear differently than its displayed content. If you add a view print formatter to a print job but do not implement this method, the view’s draw(_:) method is called to provide the content for printing.

For more information about how to implement a custom drawing routine for printed content, see Drawing and Printing Guide for iOS.

## See Also

### Formatting printed view content

func viewPrintFormatter() -> UIViewPrintFormatter

Returns a print formatter for the receiving view.

