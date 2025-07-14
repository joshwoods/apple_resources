

- UIKit
- UIAccessibilityCustomRotor
-  init(name:itemSearch:) 

Initializer

# init(name:itemSearch:)

Creates a rotor with the specified name and search block.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(
    name: String,
    itemSearch itemSearchBlock: @escaping UIAccessibilityCustomRotor.Search
)
```

## Parameters 

`name`  

The name of the rotor.

`itemSearchBlock`  

The block that provides the next or previous rotor.

## Return Value

An initialized rotor object.

## See Also

### Creating a rotor object

init(attributedName: NSAttributedString, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor with the specified name and search block.

init(systemType: UIAccessibilityCustomRotor.SystemRotorType, itemSearch: UIAccessibilityCustomRotor.Search)

Creates a rotor for the specified type of item.

