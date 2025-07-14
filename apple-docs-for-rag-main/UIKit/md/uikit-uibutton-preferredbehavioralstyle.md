

- UIKit
- UIButton
-  preferredBehavioralStyle 

Instance Property

# preferredBehavioralStyle

The preferred behavioral style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var preferredBehavioralStyle: UIBehavioralStyle { get set }
```

## Discussion

Use this property to specify the behavioral style for the button. If the value of the property is UIBehavioralStyle.automatic, use the behavioralStyle property to determine the actual style.

The default value for preferredBehavioralStyle is UIBehavioralStyle.automatic. To learn more about behavioral styles, see UIBehavioralStyle.

## See Also

### Specifying the behavioral style

var behavioralStyle: UIBehavioralStyle

The style that determines how the button behaves.

enum UIBehavioralStyle

Constants that indicate how a control behaves in apps built with Mac Catalyst.

