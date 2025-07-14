

- CarPlay
- CPMapTemplate
-  guidanceBackgroundColor 

Instance Property

# guidanceBackgroundColor

The background color the map template uses when displaying guidance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var guidanceBackgroundColor: UIColor { get set }
```

## Discussion

The system determines whether guidanceBackgroundColor meets contrast requirements, and uses the default color when the provided color doesn’t meet those requirements. The system adjusts font color to correspond with the guidance background color.

Note

The system ignores alpha values.

## See Also

### Configuring Map Templates

var automaticallyHidesNavigationBar: Bool

A Boolean value that indicates whether the template should automatically hide the navigation bar.

var hidesButtonsWithNavigationBar: Bool

A Boolean value that tells the system to hide the map buttons when hiding the navigation bar.

