

- UIKit
- UIListContentView
-  secondaryTextLayoutGuide 

Instance Property

# secondaryTextLayoutGuide

A guide for positioning the secondary text in the content view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var secondaryTextLayoutGuide: UILayoutGuide? { get }
```

## Discussion

If the configuration doesn’t specify secondary text, the value of this property is `nil`.

If you apply a new configuration without secondary text to the content view, the system removes this layout guide from the view and deactivates any constraints associated with it.

## See Also

### Managing the content layout

var textLayoutGuide: UILayoutGuide?

A guide for positioning the primary text in the content view.

var imageLayoutGuide: UILayoutGuide?

A guide for positioning the image in the content view.

