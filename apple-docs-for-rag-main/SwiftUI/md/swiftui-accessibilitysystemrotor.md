

- SwiftUI
-  AccessibilitySystemRotor 

Structure

# AccessibilitySystemRotor

Designates a Rotor that replaces one of the automatic, system-provided Rotors with a developer-provided Rotor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AccessibilitySystemRotor
```

## Topics

### Iterating through text

static var textFields: AccessibilitySystemRotor

System Rotor allowing users to iterate through all text fields.

static var boldText: AccessibilitySystemRotor

System Rotor allowing users to iterate through all the ranges of bolded text.

static var italicText: AccessibilitySystemRotor

System Rotor allowing users to iterate through all the ranges of italicized text.

static var underlineText: AccessibilitySystemRotor

System Rotor allowing users to iterate through all the ranges of underlined text.

static var misspelledWords: AccessibilitySystemRotor

System Rotor allowing users to iterate through all the ranges of mis-spelled words.

### Iterating through headings

static var headings: AccessibilitySystemRotor

System Rotor allowing users to iterate through all headings.

static func headings(level: AccessibilityHeadingLevel) -> AccessibilitySystemRotor

System Rotors allowing users to iterate through all headings, of various heading levels.

### Iterating through links

static var links: AccessibilitySystemRotor

System Rotor allowing users to iterate through all links.

static func links(visited: Bool) -> AccessibilitySystemRotor

System Rotors allowing users to iterate through links or visited links.

### Iterating through other elements

static var images: AccessibilitySystemRotor

System Rotor allowing users to iterate through all images.

static var landmarks: AccessibilitySystemRotor

System Rotor allowing users to iterate through all landmarks.

static var lists: AccessibilitySystemRotor

System Rotor allowing users to iterate through all lists.

static var tables: AccessibilitySystemRotor

System Rotor allowing users to iterate through all tables.

## Relationships

### Conforms To

- Sendable

