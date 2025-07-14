

- UIKit
- UIScreen
-  currentMode 

Instance Property

# currentMode

The current screen mode associated with the screen.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS

**iOS, iPadOS, Mac Catalyst**

``` source
@MainActor
var currentMode: UIScreenMode? { get set }
```

**tvOS**

``` source
@MainActor
var currentMode: UIScreenMode? { get }
```

## Discussion

The default value of this property is the mode containing the highest resolution supported by the screen.

On iOS, you can change the value of this property to support different resolutions as needed. For example, you might want to lower the default resolution to one that your application supports more readily. The value must be one of the values described in the availableModes property.

On tvOS, the screen mode is read-only.

## See Also

### Managing screen modes

var preferredMode: UIScreenMode?

The preferred display mode for the screen.

var availableModes: [UIScreenMode]

The display modes that can be associated with the screen.

