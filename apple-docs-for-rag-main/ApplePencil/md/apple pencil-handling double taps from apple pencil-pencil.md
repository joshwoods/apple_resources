

- Apple Pencil
-  Handling double taps from Apple Pencil 

Article

# Handling double taps from Apple Pencil

Detect and respond to double taps a person makes on Apple Pencil.

## Overview

You can use Apple Pencil interactions to allow people to access functionality in your app quickly. Double-tapping Apple Pencil lets a person perform actions such as switching between drawing tools without moving the pencil to another location on the screen.

### Register for a double tap

To respond to double taps from Apple Pencil in your app, you need to register your view to receive double-tap interactions.

- SwiftUI
- UIKit

Add an onPencilDoubleTap(perform:) view modifier to your view.

```
```

Create a UIPencilInteraction object, passing an object that implements the UIPencilInteractionDelegate protocol to the `delegate` parameter. Then, add the interaction to your view.

```
```

### Check the preferred double-tap action

A person can choose which action they prefer to perform when they double-tap Apple Pencil. They choose this systemwide preference in Settings \> Apple Pencil \> Actions \> Double Tap.

In your app, you can check the value of this preferred action for double tap.

- SwiftUI
- UIKit

To check the preferred action, use the preferredPencilDoubleTapAction environment value. For possible values, see PencilPreferredAction.

```
```

To check the preferred action, use the preferredTapAction class property on UIPencilInteraction. For possible values, see UIPencilPreferredAction.

```
```

### Choose the action to perform

When possible, perform the preferred action to provide a consistent user experience across apps that support double taps. If the preferred action doesn’t make sense in your app, consider giving people a way to choose a custom action that’s suitable for your app. For design guidance, read Human Interface Guidelines \> Apple Pencil and Scribble \> Double tap.

The following code shows a snippet from a drawing app that provides custom drawing tools. This app allows a person to configure a custom action to quickly swap to their favorite custom drawing tool instead of using the systemwide preferred action for double taps. This app also supports the preferred actions to ignore double taps, switch to the previous tool, and switch to the eraser tool.

- SwiftUI
- UIKit

```
```

```
```

## See Also

#### Related articles

#### Related reference in SwiftUI

#### Related reference in UIKit

