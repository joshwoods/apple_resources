

- SwiftUI
- View fundamentals
- View
-  Style modifiers 

API Collection

# Style modifiers

Apply built-in styles to different types of views.

## Overview

SwiftUI defines built-in styles for certain kinds of views, and chooses the appropriate style for a particular presentation context. For example, a Label might appear as an icon, a string title, or both, depending on factors like the platform, whether the view appears in a toolbar, and so on.

You can override the automatic style by using one of the style modifiers. These modifiers typically propagate through container views, so you can wrap an entire view hierarchy in a style modifier to affect all the views of the given type within the hierarchy. Some view types enable you to create custom styles, which you also apply using style modifiers.

For more information about styling views, see View styles.

## Topics

### Controls

func buttonStyle(_:)

Sets the style for buttons within this view to a button style with a custom appearance and standard interaction behavior.

func datePickerStyle&lt;S>(S) -> some View

Sets the style for date pickers within this view.

func menuStyle&lt;S>(S) -> some View

Sets the style for menus within this view.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func toggleStyle&lt;S>(S) -> some View

Sets the style for toggles in a view hierarchy.

### Indicators

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

### Text

func labelStyle&lt;S>(S) -> some View

Sets the style for labels within this view.

func textFieldStyle&lt;S>(S) -> some View

Sets the style for text fields within this view.

func textEditorStyle(some TextEditorStyle) -> some View

Sets the style for text editors within this view.

### Collections

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

func tableStyle&lt;S>(S) -> some View

Sets the style for tables within this view.

func disclosureGroupStyle&lt;S>(S) -> some View

Sets the style for disclosure groups within this view.

### Presentation

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func tabViewStyle&lt;S>(S) -> some View

Sets the style for the tab view within the current environment.

func presentedWindowStyle&lt;S>(S) -> some View

Sets the style for windows created by interacting with this view.

func presentedWindowToolbarStyle&lt;S>(S) -> some View

Sets the style for the toolbar in windows created by interacting with this view.

### Groups

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

func indexViewStyle&lt;S>(S) -> some View

Sets the style for the index view within the current environment.

## See Also

### Drawing views

Layout modifiers

Tell a view how to arrange itself within a view hierarchy by adjusting its size, position, alignment, padding, and so on.

Graphics and rendering modifiers

Affect the way the system draws a view, for example by scaling or masking a view, or by applying graphical effects.

