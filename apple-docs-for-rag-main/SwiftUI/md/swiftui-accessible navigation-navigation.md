

- SwiftUI
-  Accessible navigation 

API Collection

# Accessible navigation

Enable users to navigate to specific user interface elements using rotors.

## Overview

An accessibility rotor is a shortcut that enables users to quickly navigate to specific elements of the user interface, and, optionally, to specific ranges of text within those elements.

The system automatically provides rotors for many navigable elements, but you can supply additional rotors for specific purposes, or replace system rotors when they don’t automatically pick up off-screen elements, like those far down in a LazyVStack or a List.

For design guidance, see Accessibility in the Accessibility section of the Human Interface Guidelines.

## Topics

### Working with rotors

func accessibilityRotor(_:entries:)

Create an Accessibility Rotor with the specified user-visible label, and entries generated from the content closure.

func accessibilityRotor(_:entries:entryID:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:entries:entryLabel:)

Create an Accessibility Rotor with the specified user-visible label and entries.

func accessibilityRotor(_:textRanges:)

Create an Accessibility Rotor with the specified user-visible label and entries for each of the specified ranges. The Rotor will be attached to the current Accessibility element, and each entry will go the specified range of that element.

### Creating rotors

protocol AccessibilityRotorContent

Content within an accessibility rotor.

struct AccessibilityRotorContentBuilder

Result builder you use to generate rotor entry content.

struct AccessibilityRotorEntry

A struct representing an entry in an Accessibility Rotor.

### Replacing system rotors

struct AccessibilitySystemRotor

Designates a Rotor that replaces one of the automatic, system-provided Rotors with a developer-provided Rotor.

### Configuring rotors

func accessibilityRotorEntry&lt;ID>(id: ID, in: Namespace.ID) -> some View

Defines an explicit identifier tying an Accessibility element for this view to an entry in an Accessibility Rotor.

func accessibilityLinkedGroup&lt;ID>(id: ID, in: Namespace.ID) -> some View

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

func accessibilitySortPriority(Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

## See Also

### Accessibility

Accessibility fundamentals

Make your SwiftUI apps accessible to everyone, including people with disabilities.

Accessible appearance

Enhance the legibility of content in your app’s interface.

Accessible controls

Improve access to actions that your app can undertake.

Accessible descriptions

Describe interface elements to help people understand what they represent.

