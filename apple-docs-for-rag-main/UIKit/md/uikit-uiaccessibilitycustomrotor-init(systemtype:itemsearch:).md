

- UIKit
- UIAccessibilityCustomRotor
-  init(systemType:itemSearch:) 

Initializer

# init(systemType:itemSearch:)

Creates a rotor for the specified type of item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
init(
    systemType type: UIAccessibilityCustomRotor.SystemRotorType,
    itemSearch itemSearchBlock: @escaping UIAccessibilityCustomRotor.Search
)
```

## Parameters 

`type`  

The type of content navigated by the rotor. For a list of possible values, see UIAccessibilityCustomRotor.SystemRotorType.

`itemSearchBlock`  

The block that provides the next or previous rotor for the given type.

## Return Value

An initialized rotor object.

## See Also

### Creating a rotor object

init(attributedName: NSAttributedString, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

init(name: String, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

