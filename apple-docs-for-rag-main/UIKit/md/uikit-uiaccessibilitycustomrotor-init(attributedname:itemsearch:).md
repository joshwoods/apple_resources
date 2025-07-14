

- UIKit
- UIAccessibilityCustomRotor
-  init(attributedName:itemSearch:) 

Initializer

# init(attributedName:itemSearch:)

Creates a rotor with the specified name and search block.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
init(
    attributedName: NSAttributedString,
    itemSearch itemSearchBlock: @escaping UIAccessibilityCustomRotor.Search
)
```

## Parameters 

`attributedName`  

The name of the rotor.

`itemSearchBlock`  

The block that provides the next or previous rotor.

## Return Value

An initialized rotor object.

## See Also

### Creating a rotor object

init(name: String, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

init(systemType: UIAccessibilityCustomRotor.SystemRotorType, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor for the specified type of item.

