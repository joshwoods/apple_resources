

- UIKit
- UIContentInsetsReference
-  UIContentInsetsReference.automatic 

Case

# UIContentInsetsReference.automatic

Content insets use the system default reference point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

When you set this value on a section in a collection view, the section defaults to using the content insets reference value of the collection view.

## See Also

### Constants

case none

Content insets don’t have a reference point in relation to other insets.

case safeArea

Content insets use a reference point in relation to the safe area.

case layoutMargins

Content insets use a reference point in relation to the layout margins.

case readableContent

Content insets use a reference point in relation to the readable content guide.

