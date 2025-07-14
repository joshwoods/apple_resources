

- SwiftUI
-  AccessibilityCustomContentKey 

Structure

# AccessibilityCustomContentKey

Key used to specify the identifier and label associated with an entry of additional accessibility information.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AccessibilityCustomContentKey
```

## Overview

Use `AccessibilityCustomContentKey` and the associated modifiers taking this value as a parameter in order to simplify clearing or replacing entries of additional information that are manipulated from multiple places in your code.

## Topics

### Creating a key

init(LocalizedStringKey)

Create an `AccessibilityCustomContentKey` with the specified label.

init(_:id:)

Create an `AccessibilityCustomContentKey` with the specified label and identifier.

## Relationships

### Conforms To

- Copyable
- Equatable

## See Also

### Adding custom descriptions

func accessibilityCustomContent(_:_:importance:)

Add additional accessibility information to the view.

