

- UIKit
- UIColor
-  withProminence(\_:) 

Instance Method

# withProminence(\_:)

Returns the version of the current color that results from applying the specified prominence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
func withProminence(_ prominence: UIColor.Prominence) -> UIColor
```

## Parameters 

`prominence`  

The prominence to apply to the color. For options, see UIColor.Prominence.

## Return Value

The version of the color to display for the specified prominence.

## Discussion

Interface elements, such as text labels, can have a different level of prominence in the UI. For example, a title label appears more prominently than a subtitle or caption. When you specify a label’s color, you can pass one of the UIColor.Prominence constants to withProminence(_:) to communicate how prominently to display that color in the UI.

The following code creates a label with a secondary, vibrant red color:

```
let label = UILabel()
label.preferredVibrancy = .automatic
label.textColor = .systemRed.withProminence(.secondary) 
```

## See Also

### Working with color prominence

var prominence: UIColor.Prominence

enum Prominence

A type that indicates the prominence of a color in the interface.

