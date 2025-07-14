

- AppKit
-  NSAccessibilityCustomRotor 

Class

# NSAccessibilityCustomRotor

A context-sensitive function that helps VoiceOver users find the next instance of a related accessibility element.

macOS 10.13+

``` source
class NSAccessibilityCustomRotor
```

## Overview

Assistive apps, like VoiceOver, provide interfaces to quickly search apps for content of a specific type. For example, in a web browser, a user can quickly explore a list of navigational links or buttons using VoiceOver’s content menus.

NSAccessibilityCustomRotor provides a way for apps to vend their own content menus. For example, Pages can create a *Headings* custom rotor that allows assistive apps to search the Pages document for all headings.

## Topics

### Creating a Rotor

init(label: String, itemSearchDelegate: any NSAccessibilityCustomRotorItemSearchDelegate)

Creates a custom rotor with the specified label and item search delegate.

init(rotorType: NSAccessibilityCustomRotor.RotorType, itemSearchDelegate: any NSAccessibilityCustomRotorItemSearchDelegate)

Creates a custom rotor with the specified rotor type and item search delegate.

### Navigating to the Next Item

var itemSearchDelegate: (any NSAccessibilityCustomRotorItemSearchDelegate)?

The delegate for finding the next item result.

protocol NSAccessibilityCustomRotorItemSearchDelegate

A delegate for a custom rotor that finds the next item result after performing a search with the specified search parameters.

### Loading the Item

var itemLoadingDelegate: (any NSAccessibilityElementLoading)?

The delegate for loading item results that don’t have a backing UI element at loading time.

protocol NSAccessibilityElementLoading

A role-based protocol that declares the minimum interface necessary for an accessibility element to support loading.

### Getting the Rotor Type

var type: NSAccessibilityCustomRotor.RotorType

The type of content that the rotor represents.

enum RotorType

Constants that indicate the type of content that the rotor represents.

### Identifying the Rotor

var label: String

The localized label that assistive apps use to describe the custom rotor.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Assigning Rotors

func accessibilityCustomRotors() -> [NSAccessibilityCustomRotor]

Returns the custom rotors of the current accessibility element.

**Required**

func setAccessibilityCustomRotors([NSAccessibilityCustomRotor])

Sets the custom rotors of the current accessibility element.

**Required**

