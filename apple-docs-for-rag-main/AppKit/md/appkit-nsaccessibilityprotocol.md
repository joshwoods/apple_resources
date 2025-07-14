

- AppKit
-  NSAccessibilityProtocol 

Protocol

# NSAccessibilityProtocol

The complete list of properties and methods for accessible elements.

macOS

``` source
protocol NSAccessibilityProtocol : NSObjectProtocol
```

## Overview

To be accessible, an app must provide information to the assistive app about its user interface and capabilities. There are three ways that apps and assistive apps interact:

- Informational properties. NSAccessibilityProtocol defines a number of properties that provide information about your view or control. If you’re working with a subclass of a standard AppKit view or control, you can either set the desired property or override its getters and setters. By default, overriding only the getter tells the assistive app that it has read-only access to the property. Overriding the setter tells the assistive app that it also has write access to the property.

- Action methods. NSAccessibilityProtocol also defines a number of methods that simulate button presses, mouse clicks, and selections in your view or control. By implementing these methods, you give assistive apps the ability to drive your view or control.

- Notifications. Your view or control may need to let the assistive app know when changes occur. NSAccessibility.Notification defines a number of notifications that you can send using the post(element:notification:) method. The role-specific protocols don’t include these notifications; however, standard AppKit controls already send appropriate messages for their standard usage patterns. You typically need to send your own notifications only when you’re creating a custom control or when you’re using a standard control in a nonstandard way.

If you’re using standard AppKit user interface elements, much of the work has been done for you. AppKit views and controls adopt the NSAccessibilityProtocol protocol by default. In particular, NSView, NSWindow, NSCell, and NSDrawer provide a default implementation for all the properties and methods in this protocol. In some cases, you may need to modify these default values to better represent your app, to provide additional context, or to modify the user’s flow through the app.

If you’re using custom view or control subclasses, you need to add the appropriate informational properties, action methods, and notifications. You do this by adopting a role-specific protocol instead of NSAccessibilityProtocol. See Custom Controls.

If you’re using custom user interface elements that don’t inherit from NSView or one of the other accessibility-enabled AppKit classes, subclass the NSAccessibilityElement class instead of adopting instead of NSAccessibilityProtocol.

### Customizing User Interface Elements

Often, you can adjust how an assistive app interacts with your user interface element without creating a custom subclass. If a user interface element inherits from NSView or one of the other accessibility-enabled AppKit classes, you can customize it by:

- Setting its accessibility values using any of the setter methods in the NSAccessibilityProtocol protocol.

- Overriding any of the properties or methods in the NSAccessibilityProtocol protocol with a custom implementation.

If you override a getter method, the system lets assistive apps call your getter. This can be particularly useful when managing dynamic properties because you can calculate their current value on demand instead of trying to update the property in response to a change.

If you override a setter method, the system lets assistive apps both read and modify that property.

You can control which accessor methods the assistive app can use by overriding isAccessibilitySelectorAllowed(_:). Return true if the assistive app can call the selector; otherwise, return false.

## Topics

### Configuring Accessibility

func isAccessibilityElement() -> Bool

Returns a Boolean value that determines whether the accessibility element participates in the accessibility hierarchy.

**Required**

func setAccessibilityElement(Bool)

Sets a Boolean value that determines whether the accessibility element participates in the accessibility hierarchy.

**Required**

func isAccessibilityEnabled() -> Bool

Returns a Boolean value that determines whether the accessibility element responds to user events.

**Required**

func setAccessibilityEnabled(Bool)

Sets a Boolean value that determines whether the accessibility element responds to user events.

**Required**

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func setAccessibilityFrame(NSRect)

Sets the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityHelp() -> String?

Returns the help text for the accessibility element.

**Required**

func setAccessibilityHelp(String?)

Sets the help text for the accessibility element.

**Required**

func accessibilityLabel() -> String?

Returns a short description of the accessibility element.

**Required**

func setAccessibilityLabel(String?)

Sets a short description of the accessibility element.

**Required**

func accessibilityTitle() -> String?

Returns the title of the accessibility element—for example, a button’s visible text.

**Required**

func setAccessibilityTitle(String?)

Sets the title of the accessibility element.

**Required**

func accessibilityValue() -> Any?

Returns the accessibility element’s value.

**Required**

func setAccessibilityValue(Any?)

Sets the accessibility element’s value.

**Required**

func isAccessibilitySelectorAllowed(Selector) -> Bool

Returns a Boolean value that indicates whether assistive apps can invoke the specified selector on the accessibility element.

**Required**

### Setting Content and Values

func accessibilityContents() -> [Any]?

Returns the contents of the current accessibility element.

**Required**

func setAccessibilityContents([Any]?)

Sets the contents of the current accessibility element.

**Required**

func accessibilityCriticalValue() -> Any?

Returns the critical value for the level indicator.

**Required**

func setAccessibilityCriticalValue(Any?)

Sets the critical value for the level indicator.

**Required**

func accessibilityIdentifier() -> String?

Returns the accessibility element’s identity.

**Required**

func setAccessibilityIdentifier(String?)

Sets the accessibility element’s identity.

**Required**

func accessibilityMaxValue() -> Any?

Returns the maximum value for the accessibility element.

**Required**

func setAccessibilityMaxValue(Any?)

Sets the maximum value for the accessibility element.

**Required**

func accessibilityMinValue() -> Any?

Returns the minimum value for the accessibility element.

**Required**

func setAccessibilityMinValue(Any?)

Sets the minimum value for the accessibility element.

**Required**

func accessibilityOrientation() -> NSAccessibilityOrientation

Returns the orientation of the accessibility element.

**Required**

func setAccessibilityOrientation(NSAccessibilityOrientation)

Sets the orientation of the accessibility element.

**Required**

func isAccessibilityProtectedContent() -> Bool

Returns a Boolean value that determines whether the accessibility element contains protected content.

**Required**

func setAccessibilityProtectedContent(Bool)

Sets a Boolean value that determines whether the accessibility element contains protected content.

**Required**

func isAccessibilitySelected() -> Bool

Returns a Boolean value that determines whether the accessibility element is currently in a selected state.

**Required**

func setAccessibilitySelected(Bool)

Sets a Boolean value that determines whether the accessibility element is currently in a selected state.

**Required**

func accessibilityURL() -> URL?

Returns the URL for the accessibility element.

**Required**

func setAccessibilityURL(URL?)

Sets the URL for the accessibility element.

**Required**

func accessibilityValueDescription() -> String?

Returns the human-readable description of the accessibility element’s value.

**Required**

func setAccessibilityValueDescription(String?)

Sets the human-readable description of the accessibility element’s value.

**Required**

func accessibilityWarningValue() -> Any?

Returns the warning value for the level indicator.

**Required**

func setAccessibilityWarningValue(Any?)

Sets the warning value for the level indicator.

**Required**

enum NSAccessibilityOrientation

Values that indicate the orientation of accessibility elements, such as scroll bars and split views.

### Determining Relationships

func accessibilityChildren() -> [Any]?

Returns the child accessibility elements in the accessibility hierarchy.

**Required**

func setAccessibilityChildren([Any]?)

Sets the child accessibility elements in the accessibility hierarchy.

**Required**

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

Returns the array of child accessibility elements in order for linear navigation.

**Required**

func setAccessibilityChildrenInNavigationOrder([any NSAccessibilityElementProtocol]?)

Sets the array of child accessibility elements in order for linear navigation.

**Required**

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

func setAccessibilityParent(Any?)

Sets the accessibility element’s parent in the accessibility hierarchy.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the accessibility element’s currently selected children.

**Required**

func setAccessibilitySelectedChildren([Any]?)

Sets the accessibility element’s currently selected children.

**Required**

func accessibilityTopLevelUIElement() -> Any?

Returns the top-level element that contains the accessibility element.

**Required**

func setAccessibilityTopLevelUIElement(Any?)

Sets the top-level element that contains the accessibility element.

**Required**

func accessibilityVisibleChildren() -> [Any]?

Returns the accessibility element’s visible child accessibility elements.

**Required**

func setAccessibilityVisibleChildren([Any]?)

Sets the accessibility element’s visible child accessibility elements.

**Required**

### Setting the Focus

func accessibilityApplicationFocusedUIElement() -> Any?

Returns the child accessibility element with the current focus.

**Required**

func setAccessibilityApplicationFocusedUIElement(Any?)

Sets the child accessibility element with the current focus.

**Required**

func isAccessibilityFocused() -> Bool

Returns a Boolean value that determines whether the accessibility element has the keyboard focus.

**Required**

func setAccessibilityFocused(Bool)

Sets a Boolean value that determines whether the accessibility element has the keyboard focus.

**Required**

func accessibilityFocusedWindow() -> Any?

Returns the child window with the current focus.

**Required**

func setAccessibilityFocusedWindow(Any?)

Sets the child window with the current focus.

**Required**

func accessibilitySharedFocusElements() -> [Any]?

Returns the array of elements that shares the keyboard focus with the accessibility element.

**Required**

func setAccessibilitySharedFocusElements([Any]?)

Sets the array of elements that shares the keyboard focus with the accessibility element.

**Required**

### Assigning Roles

func isAccessibilityRequired() -> Bool

Returns a Boolean value that determines whether the accessibility element must have content for successful submission of a form.

**Required**

func setAccessibilityRequired(Bool)

Sets a Boolean value that determines whether the accessibility element must have content for successful submission of a form.

**Required**

func accessibilityRole() -> NSAccessibility.Role?

Returns the type of interface element that the accessibility element represents.

**Required**

func setAccessibilityRole(NSAccessibility.Role?)

Sets the type of interface element that the accessibility element represents.

**Required**

func accessibilityRoleDescription() -> String?

Returns a localized, human-intelligible description of the accessibility element’s role, such as *radio button*.

**Required**

func setAccessibilityRoleDescription(String?)

Sets the localized, human-intelligible description of the accessibility element’s role, such as *radio button*.

**Required**

func accessibilitySubrole() -> NSAccessibility.Subrole?

Returns the specialized interface element type that the accessibility element represents.

**Required**

func setAccessibilitySubrole(NSAccessibility.Subrole?)

Sets the specialized interface element type that the accessibility element represents.

**Required**

struct Role

Values that describe types of objects that accessibility elements represent.

struct Subrole

Values that describe specialized object subtypes that accessibility elements represent.

### Assigning Actions

func accessibilityCustomActions() -> [NSAccessibilityCustomAction]?

Returns the custom actions of the current accessibility element.

**Required**

func setAccessibilityCustomActions([NSAccessibilityCustomAction]?)

Sets the custom actions of the current accessibility element.

**Required**

class NSAccessibilityCustomAction

A custom action to perform on an accessible object.

### Assigning Rotors

func accessibilityCustomRotors() -> [NSAccessibilityCustomRotor]

Returns the custom rotors of the current accessibility element.

**Required**

func setAccessibilityCustomRotors([NSAccessibilityCustomRotor])

Sets the custom rotors of the current accessibility element.

**Required**

class NSAccessibilityCustomRotor

A context-sensitive function that helps VoiceOver users find the next instance of a related accessibility element.

### Configuring Text Elements

func accessibilityInsertionPointLineNumber() -> Int

Returns the line number that contains the insertion point.

**Required**

func setAccessibilityInsertionPointLineNumber(Int)

Sets the line number that contains the insertion point.

**Required**

func accessibilityNumberOfCharacters() -> Int

Returns the number of characters in the text.

**Required**

func setAccessibilityNumberOfCharacters(Int)

Sets the number of characters in the text.

**Required**

func accessibilityPlaceholderValue() -> String?

Returns the placeholder value for the accessibility element.

**Required**

func setAccessibilityPlaceholderValue(String?)

Sets the placeholder value for the accessibility element.

**Required**

func accessibilitySelectedText() -> String?

Returns the currently selected text.

**Required**

func setAccessibilitySelectedText(String?)

Sets the currently selected text.

**Required**

func accessibilitySelectedTextRange() -> NSRange

Returns the range of the currently selected text.

**Required**

func setAccessibilitySelectedTextRange(NSRange)

Sets the range of the currently selected text.

**Required**

func accessibilitySelectedTextRanges() -> [NSValue]?

Returns an array of ranges for the currently selected text.

**Required**

func setAccessibilitySelectedTextRanges([NSValue]?)

Sets an array of ranges for the currently selected text.

**Required**

func accessibilitySharedCharacterRange() -> NSRange

Returns the range of characters that the accessibility element displays.

**Required**

func setAccessibilitySharedCharacterRange(NSRange)

Sets the range of characters that the accessibility element displays.

**Required**

func accessibilitySharedTextUIElements() -> [Any]?

Returns the other elements that share text with the accessibility element.

**Required**

func setAccessibilitySharedTextUIElements([Any]?)

Sets the other elements that share text with the accessibility element.

**Required**

func accessibilityVisibleCharacterRange() -> NSRange

Returns the range of visible characters in the document.

**Required**

func setAccessibilityVisibleCharacterRange(NSRange)

Sets the range of visible characters in the document.

**Required**

func accessibilityString(for: NSRange) -> String?

Returns the substring for the specified range.

**Required**

func accessibilityAttributedString(for: NSRange) -> NSAttributedString?

Returns the attributed substring for the specified range of characters.

**Required**

func accessibilityRTF(for: NSRange) -> Data?

Returns the rich text format (RTF) data that describes the specified range of characters.

**Required**

func accessibilityFrame(for: NSRange) -> NSRect

Returns the rectangle that encloses the specified range of characters.

**Required**

func accessibilityLine(for: Int) -> Int

Returns the line number for the line that contains the specified character index.

**Required**

func accessibilityRange(for: Int) -> NSRange

Returns the range of characters for the glyph that includes the specified character.

**Required**

func accessibilityStyleRange(for: Int) -> NSRange

Returns a range of characters that all have the same style as the specified character.

**Required**

func accessibilityRange(forLine: Int) -> NSRange

Returns the range of characters in the specified line.

**Required**

func accessibilityRange(for: NSPoint) -> NSRange

Returns the range of characters for the glyph at the specified point.

**Required**

### Configuring Windows

func accessibilityActivationPoint() -> NSPoint

Returns the activation point for the user interface element.

**Required**

func setAccessibilityActivationPoint(NSPoint)

Sets the activation point for the user interface element.

**Required**

func isAccessibilityAlternateUIVisible() -> Bool

Returns the Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

**Required**

func setAccessibilityAlternateUIVisible(Bool)

Sets the Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

**Required**

func accessibilityCancelButton() -> Any?

Returns the child accessibility element that represents the window’s cancel button.

**Required**

func setAccessibilityCancelButton(Any?)

Sets the child accessibility element that represents the window’s cancel button.

**Required**

func accessibilityCloseButton() -> Any?

Returns the child accessibility element that represents the window’s close button.

**Required**

func setAccessibilityCloseButton(Any?)

Sets the child accessibility element that represents the window’s close button.

**Required**

func accessibilityDefaultButton() -> Any?

Returns the child accessibility element that represents the window’s default button.

**Required**

func setAccessibilityDefaultButton(Any?)

Sets the child accessibility element that represents the window’s default button.

**Required**

func accessibilityFullScreenButton() -> Any?

Returns the child accessibility element that represents the window’s full-screen button.

**Required**

func setAccessibilityFullScreenButton(Any?)

Sets the child accessibility element that represents the window’s full-screen button.

**Required**

func accessibilityGrowArea() -> Any?

Returns the child accessibility element that represents the window’s grow area.

**Required**

func setAccessibilityGrowArea(Any?)

Sets the child accessibility element that represents the window’s grow area.

**Required**

func isAccessibilityMain() -> Bool

Returns a Boolean value that determines whether the window is the app’s main window.

**Required**

func setAccessibilityMain(Bool)

Sets a Boolean value that determines whether the window is the app’s main window.

**Required**

func accessibilityMinimizeButton() -> Any?

Returns the child accessibility element that represents the window’s minimize button.

**Required**

func setAccessibilityMinimizeButton(Any?)

Sets the child accessibility element that represents the window’s minimize button.

**Required**

func isAccessibilityMinimized() -> Bool

Returns the Boolean value that determines whether the window is in a minimized state.

**Required**

func setAccessibilityMinimized(Bool)

Sets the Boolean value that determines whether the window is in a minimized state.

**Required**

func isAccessibilityModal() -> Bool

Returns a Boolean value that determines whether the window is modal.

**Required**

func setAccessibilityModal(Bool)

Sets a Boolean value that determines whether the window is modal.

**Required**

func accessibilityProxy() -> Any?

Returns the child accessibility element that represents the window’s proxy icon.

**Required**

func setAccessibilityProxy(Any?)

Sets the child accessibility element that represents the window’s proxy icon.

**Required**

func accessibilityShownMenu() -> Any?

Returns the menu currently displaying for the accessibility element.

**Required**

func setAccessibilityShownMenu(Any?)

Sets the menu currently displaying for the accessibility element.

**Required**

func accessibilityToolbarButton() -> Any?

Returns the child accessibility element that represents the window’s toolbar button.

**Required**

func setAccessibilityToolbarButton(Any?)

Sets the child accessibility element that represents the window’s toolbar button.

**Required**

func accessibilityWindow() -> Any?

Returns the window that contains the accessibility element.

**Required**

func setAccessibilityWindow(Any?)

Sets the window that contains the accessibility element.

**Required**

func accessibilityZoomButton() -> Any?

Returns the child accessibility element that represents the window’s zoom button.

**Required**

func setAccessibilityZoomButton(Any?)

Sets the child accessibility element that represents the window’s zoom button.

**Required**

### Managing Apps

func accessibilityExtrasMenuBar() -> Any?

Returns the icon for the app’s menu bar extra.

**Required**

func setAccessibilityExtrasMenuBar(Any?)

Sets the icon for the app’s menu bar extra.

**Required**

func isAccessibilityFrontmost() -> Bool

Returns a Boolean value that determines whether the app is the frontmost app.

**Required**

func setAccessibilityFrontmost(Bool)

Sets a Boolean value that determines whether the app is the frontmost app.

**Required**

func isAccessibilityHidden() -> Bool

Returns a Boolean value that determines whether the app is in a hidden state.

**Required**

func setAccessibilityHidden(Bool)

Sets a Boolean value that determines whether the app is in a hidden state.

**Required**

func accessibilityMainWindow() -> Any?

Returns the app’s main window.

**Required**

func setAccessibilityMainWindow(Any?)

Sets the app’s main window.

**Required**

func accessibilityMenuBar() -> Any?

Returns the app’s menu bar.

**Required**

func setAccessibilityMenuBar(Any?)

Sets the app’s menu bar.

**Required**

func accessibilityWindows() -> [Any]?

Returns an array that contains all the app’s windows.

**Required**

func setAccessibilityWindows([Any]?)

Sets the array that contains all the app’s windows.

**Required**

### Configuring Grid Views

func accessibilityColumnCount() -> Int

Returns the number of columns in the accessibility element’s grid.

**Required**

func setAccessibilityColumnCount(Int)

Sets the number of columns in the accessibility element’s grid.

**Required**

func isAccessibilityOrderedByRow() -> Bool

Returns a Boolean value that determines whether the accessibility element’s grid is in row major order or in column major order.

**Required**

func setAccessibilityOrderedByRow(Bool)

Sets a Boolean value that determines whether the element’s grid is in row major order or in column major order.

**Required**

func accessibilityRowCount() -> Int

Returns the number of rows in the accessibility element’s grid.

**Required**

func setAccessibilityRowCount(Int)

Sets the number of rows in the accessibility element’s grid.

**Required**

### Configuring Scroll Views

func accessibilityHorizontalScrollBar() -> Any?

Returns the horizontal scroll bar for the scroll view.

**Required**

func setAccessibilityHorizontalScrollBar(Any?)

Sets the horizontal scroll bar for the scroll view.

**Required**

func accessibilityVerticalScrollBar() -> Any?

Returns the vertical scroll bar for the scroll view.

**Required**

func setAccessibilityVerticalScrollBar(Any?)

Sets the vertical scroll bar for the scroll view.

**Required**

### Configuring Table and Outline Views

func accessibilityColumnHeaderUIElements() -> [Any]?

Returns the column header accessibility elements for the table or outline.

**Required**

func setAccessibilityColumnHeaderUIElements([Any]?)

Sets the column header accessibility elements for the table or outline.

**Required**

func accessibilityColumns() -> [Any]?

Returns the column accessibility elements for the table or outline.

**Required**

func setAccessibilityColumns([Any]?)

Sets the column accessibility elements for the table or outline.

**Required**

func accessibilityColumnTitles() -> [Any]?

Returns the column titles for the accessibility element.

**Required**

func setAccessibilityColumnTitles([Any]?)

Sets the column titles for the accessibility element.

**Required**

func isAccessibilityExpanded() -> Bool

Returns a Boolean value that determines whether the accessibility element is in an expanded state.

**Required**

func setAccessibilityExpanded(Bool)

Sets a Boolean value that determines whether accessibility element is in an expanded state.

**Required**

func accessibilityHeader() -> Any?

Returns the header for the table view.

**Required**

func setAccessibilityHeader(Any?)

Sets the header for the table view.

**Required**

func accessibilityIndex() -> Int

Returns the index of the row or column that the accessibility element represents.

**Required**

func setAccessibilityIndex(Int)

Sets the index of the row or column that the accessibility element represents.

**Required**

func accessibilityRowHeaderUIElements() -> [Any]?

Returns the row header accessibility elements for the table or outline.

**Required**

func setAccessibilityRowHeaderUIElements([Any]?)

Sets the row header accessibility elements for the table or outline.

**Required**

func accessibilityRows() -> [Any]?

Returns the row accessibility elements for the table or outline.

**Required**

func setAccessibilityRows([Any]?)

Sets the row accessibility elements for the table or outline.

**Required**

func accessibilitySelectedColumns() -> [Any]?

Returns the currently selected columns for the table or outline.

**Required**

func setAccessibilitySelectedColumns([Any]?)

Sets the currently selected columns for the table or outline.

**Required**

func accessibilitySelectedRows() -> [Any]?

Returns the currently selected rows for the table or outline.

**Required**

func setAccessibilitySelectedRows([Any]?)

Sets the currently selected rows for the table or outline.

**Required**

func accessibilitySortDirection() -> NSAccessibilitySortDirection

Returns the accessibility element’s sort direction.

**Required**

func setAccessibilitySortDirection(NSAccessibilitySortDirection)

Sets the accessibility element’s sort direction.

**Required**

func accessibilityVisibleColumns() -> [Any]?

Returns the visible columns for the table or outline.

**Required**

func setAccessibilityVisibleColumns([Any]?)

Sets the visible columns for the table or outline.

**Required**

func accessibilityVisibleRows() -> [Any]?

Returns the visible rows for the table or outline.

**Required**

func setAccessibilityVisibleRows([Any]?)

Sets the visible rows for the table or outline.

**Required**

enum NSAccessibilitySortDirection

Values that indicate the sort direction of a column.

### Configuring Outline Rows

func isAccessibilityDisclosed() -> Bool

Returns a Boolean value that determines whether the row is disclosing other rows.

**Required**

func setAccessibilityDisclosed(Bool)

Sets a Boolean value that determines whether the row is disclosing other rows.

**Required**

func accessibilityDisclosedByRow() -> Any?

Returns the row disclosing the current row.

**Required**

func setAccessibilityDisclosedByRow(Any?)

Sets the row disclosing the current row.

**Required**

func accessibilityDisclosedRows() -> Any?

Returns the rows that the current row discloses.

**Required**

func setAccessibilityDisclosedRows(Any?)

Sets the rows that the current row discloses.

**Required**

func accessibilityDisclosureLevel() -> Int

Returns the indention level for the row.

**Required**

func setAccessibilityDisclosureLevel(Int)

Sets the indention level for the row.

**Required**

### Configuring Cell-Based Tables

func accessibilityColumnIndexRange() -> NSRange

Returns the column index range of the cell.

**Required**

func setAccessibilityColumnIndexRange(NSRange)

Sets the column index range of the cell.

**Required**

func accessibilityRowIndexRange() -> NSRange

Returns the row index range of the cell.

**Required**

func setAccessibilityRowIndexRange(NSRange)

Sets the row index range of the cell.

**Required**

func accessibilitySelectedCells() -> [Any]?

Returns the currently selected cells for the table.

**Required**

func setAccessibilitySelectedCells([Any]?)

Sets the currently selected cells for the table.

**Required**

func accessibilityVisibleCells() -> [Any]?

Returns the visible cells for the table.

**Required**

func setAccessibilityVisibleCells([Any]?)

Sets the visible cells for the table.

**Required**

func accessibilityCell(forColumn: Int, row: Int) -> Any?

Returns the cell at the specified column and row.

**Required**

### Configuring Layout

func accessibilityHandles() -> [Any]?

Returns the drag handle elements for the layout item element.

**Required**

func setAccessibilityHandles([Any]?)

Sets the drag handle accessibility elements for the layout item element.

**Required**

func accessibilityHorizontalUnits() -> NSAccessibilityUnits

Returns the units that the layout area uses for horizontal values.

**Required**

func setAccessibilityHorizontalUnits(NSAccessibilityUnits)

Sets the units that the layout area uses for horizontal values.

**Required**

func accessibilityHorizontalUnitDescription() -> String?

Returns the description of the layout area’s horizontal units.

**Required**

func setAccessibilityHorizontalUnitDescription(String?)

Sets the description of the layout area’s horizontal units.

**Required**

func accessibilityVerticalUnits() -> NSAccessibilityUnits

Returns the units that the layout area uses for vertical values.

**Required**

func setAccessibilityVerticalUnits(NSAccessibilityUnits)

Sets the units that the layout area uses for vertical values.

**Required**

func accessibilityVerticalUnitDescription() -> String?

Returns the description of the layout area’s vertical units.

**Required**

func setAccessibilityVerticalUnitDescription(String?)

Sets the description of the layout area’s vertical units.

**Required**

func accessibilityLayoutPoint(forScreenPoint: NSPoint) -> NSPoint

Converts the provided point in screen coordinates to a point in the layout area’s coordinate system.

**Required**

func accessibilityLayoutSize(forScreenSize: NSSize) -> NSSize

Converts the provided size in screen coordinates to a size in the layout area’s coordinate system.

**Required**

func accessibilityScreenPoint(forLayoutPoint: NSPoint) -> NSPoint

Converts the provided point in the layout area’s coordinates to a point in the screen’s coordinate system.

**Required**

func accessibilityScreenSize(forLayoutSize: NSSize) -> NSSize

Converts the provided size in the layout area’s coordinates to a size in the screen’s coordinate system.

**Required**

### Configuring Sliders

func accessibilityAllowedValues() -> [NSNumber]?

Returns the allowed values for the slider accessibility element.

**Required**

func setAccessibilityAllowedValues([NSNumber]?)

Sets the allowed values for the slider accessibility element.

**Required**

func accessibilityLabelUIElements() -> [Any]?

Returns the child label elements for the slider accessibility element.

**Required**

func setAccessibilityLabelUIElements([Any]?)

Sets the child label elements for the slider accessibility element.

**Required**

func accessibilityLabelValue() -> Float

Returns the value of the label accessibility element.

**Required**

func setAccessibilityLabelValue(Float)

Sets the value of the label accessibility element.

**Required**

### Configuring Split Views

func accessibilityNextContents() -> [Any]?

Returns the contents that follow the divider accessibility element.

**Required**

func setAccessibilityNextContents([Any]?)

Sets the contents that follow the divider accessibility element.

**Required**

func accessibilityPreviousContents() -> [Any]?

Returns the contents that precede the divider accessibility element.

**Required**

func setAccessibilityPreviousContents([Any]?)

Sets the contents that precede the divider accessibility element.

**Required**

func accessibilitySplitters() -> [Any]?

Returns an array that contains the views and splitter bar from the split view.

**Required**

func setAccessibilitySplitters([Any]?)

Sets the array that contains the views and splitter bar from the split view.

**Required**

### Configuring Tabs and Toolbars

func accessibilityOverflowButton() -> Any?

Returns the overflow button for the toolbar.

**Required**

func setAccessibilityOverflowButton(Any?)

Sets the overflow button for the toolbar.

**Required**

func accessibilityTabs() -> [Any]?

Returns the tab accessibility elements for the tab view.

**Required**

func setAccessibilityTabs([Any]?)

Sets the tab accessibility elements for the tab view.

**Required**

### Configuring Ruler Views

func accessibilityMarkerGroupUIElement() -> Any?

Returns the user interface element that functions as a marker group for the ruler accessibility element.

**Required**

func setAccessibilityMarkerGroupUIElement(Any?)

Sets the user interface element that functions as a marker group for the ruler accessibility element.

**Required**

func accessibilityMarkerTypeDescription() -> String?

Returns the human-readable description of the marker type.

**Required**

func setAccessibilityMarkerTypeDescription(String?)

Sets the human-readable description of the marker type.

**Required**

func accessibilityMarkerUIElements() -> [Any]?

Returns the array of marker accessibility elements for the ruler.

**Required**

func setAccessibilityMarkerUIElements([Any]?)

Sets the array of marker accessibility elements for the ruler.

**Required**

func accessibilityMarkerValues() -> Any?

Returns the marker values for the ruler.

**Required**

func setAccessibilityMarkerValues(Any?)

Sets the marker values for the ruler.

**Required**

func accessibilityRulerMarkerType() -> NSAccessibilityRulerMarkerType

Returns the type of markers for the ruler.

**Required**

func setAccessibilityRulerMarkerType(NSAccessibilityRulerMarkerType)

Sets the type of markers for the ruler.

**Required**

func accessibilityUnits() -> NSAccessibilityUnits

Returns the units for the ruler.

**Required**

func setAccessibilityUnits(NSAccessibilityUnits)

Sets the units used for the ruler.

**Required**

func accessibilityUnitDescription() -> String?

Returns the human-readable description of the ruler’s units.

**Required**

func setAccessibilityUnitDescription(String?)

Sets the human-readable description of the ruler’s units.

**Required**

enum NSAccessibilityRulerMarkerType

Values that indicate the marker type of an accessibility element.

enum NSAccessibilityUnits

Values that indicate the unit values of a ruler or layout area.

### Managing Documents and Editing

func accessibilityDocument() -> String?

Returns the URL for the file that the accessibility element represents.

**Required**

func setAccessibilityDocument(String?)

Sets the URL for the file that the accessibility element represents.

**Required**

func isAccessibilityEdited() -> Bool

Returns a Boolean value that indicates whether the accessibility element is in an edited state.

**Required**

func setAccessibilityEdited(Bool)

Sets a Boolean value that indicates whether the accessibility element is in an edited state.

**Required**

func accessibilityFilename() -> String?

Returns the filename for the file that the accessibility element represents.

**Required**

func setAccessibilityFilename(String?)

Sets the filename for the file that the accessibility element represents.

**Required**

### Configuring Linkage Elements

func accessibilityLinkedUIElements() -> [Any]?

Returns the elements that have links with the accessibility element.

**Required**

func setAccessibilityLinkedUIElements([Any]?)

Sets the elements that have links with the accessibility element.

**Required**

func accessibilityServesAsTitleForUIElements() -> [Any]?

Returns the list of elements that the accessibility element is a title for.

**Required**

func setAccessibilityServesAsTitleForUIElements([Any]?)

Sets the list of elements that the accessibility element is a title for.

**Required**

func accessibilityTitleUIElement() -> Any?

Returns the static text element that represents the accessibility element’s title.

**Required**

func setAccessibilityTitleUIElement(Any?)

Sets the static text element that represents the accessibility element’s title.

**Required**

### Configuring Search

func accessibilityClearButton() -> Any?

Returns the clear button for the search field.

**Required**

func setAccessibilityClearButton(Any?)

Sets the clear button for the search field.

**Required**

func accessibilitySearchButton() -> Any?

Returns the search button for the search field.

**Required**

func setAccessibilitySearchButton(Any?)

Sets the search button for the search field.

**Required**

func accessibilitySearchMenu() -> Any?

Returns the search menu for the search field.

**Required**

func setAccessibilitySearchMenu(Any?)

Sets the search menu for the search field.

**Required**

### Confirming and Canceling Operations

func accessibilityPerformCancel() -> Bool

Cancels the current operation.

**Required**

func accessibilityPerformConfirm() -> Bool

Simulates pressing Return in the accessibility element.

**Required**

### Selecting Elements

func accessibilityPerformPick() -> Bool

Selects the accessibility element.

**Required**

func accessibilityPerformPress() -> Bool

Simulates clicking the accessibility element.

**Required**

### Showing User Interface Elements

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func accessibilityPerformShowMenu() -> Bool

Displays the menu accessibility element.

**Required**

func accessibilityPerformRaise() -> Bool

Brings the window to the front.

**Required**

### Incrementing, Decrementing, and Deleting Values

func accessibilityIncrementButton() -> Any?

Returns the increment button for the stepper accessibility element.

**Required**

func setAccessibilityIncrementButton(Any?)

Sets the increment button for the stepper accessibility element.

**Required**

func accessibilityDecrementButton() -> Any?

Returns the decrement button for the stepper accessibility element.

**Required**

func setAccessibilityDecrementButton(Any?)

Sets the decrement button for the stepper accessibility element.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the accessibility element’s value.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the accessibility element’s value.

**Required**

func accessibilityPerformDelete() -> Bool

Deletes the accessibility element’s value.

**Required**

### Managing Notifications

Notifications alert assistive apps to changes in the user interface’s state.

static func post(element: Any, notification: NSAccessibility.Notification)

Sends a notification to any observing assistive apps.

static func post(element: Any, notification: NSAccessibility.Notification, userInfo: [NSAccessibility.NotificationUserInfoKey : Any]?)

Sends a notification and an optional user info dictionary to any observing assistive apps.

struct Notification

The name of the notification.

struct NotificationUserInfoKey

The key in the user info dictionary for a notification.

### Handling Errors

static let ErrorCodeExceptionInfo: String

An integer error code for debugging.

### Instance Properties

struct NSAccessibility

A namespace for accessibility symbols for AppKit apps.

### Instance Methods

func accessibilityAttributedUserInputLabels() -> [NSAttributedString]?

**Required**

func accessibilityUserInputLabels() -> [String]?

**Required**

func setAccessibilityAttributedUserInputLabels([NSAttributedString]?)

**Required**

func setAccessibilityUserInputLabels([String]?)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSAccessibilityElement
- NSActionCell
- NSApplication
- NSBox
- NSBrowser
- NSBrowserCell
- NSButton
- NSButtonCell
- NSCell
- NSClipView
- NSCollectionView
- NSColorPanel
- NSColorWell
- NSComboBox
- NSComboBoxCell
- NSComboButton
- NSControl
- NSDatePicker
- NSDatePickerCell
- NSDrawer
- NSFontPanel
- NSForm
- NSFormCell
- NSGridView
- NSImageCell
- NSImageView
- NSLevelIndicator
- NSLevelIndicatorCell
- NSMatrix
- NSMenu
- NSMenuItem
- NSMenuItemCell
- NSOpenGLView
- NSOpenPanel
- NSOutlineView
- NSPanel
- NSPathCell
- NSPathComponentCell
- NSPathControl
- NSPopUpButton
- NSPopUpButtonCell
- NSPopover
- NSPredicateEditor
- NSProgressIndicator
- NSRuleEditor
- NSRulerView
- NSSavePanel
- NSScrollView
- NSScroller
- NSScrubber
- NSScrubberArrangedView
- NSScrubberImageItemView
- NSScrubberItemView
- NSScrubberSelectionView
- NSScrubberTextItemView
- NSSearchField
- NSSearchFieldCell
- NSSecureTextField
- NSSecureTextFieldCell
- NSSegmentedCell
- NSSegmentedControl
- NSSlider
- NSSliderAccessory
- NSSliderCell
- NSSplitView
- NSStackView
- NSStatusBarButton
- NSStepper
- NSStepperCell
- NSSwitch
- NSTabView
- NSTableCellView
- NSTableHeaderCell
- NSTableHeaderView
- NSTableRowView
- NSTableView
- NSText
- NSTextAttachmentCell
- NSTextField
- NSTextFieldCell
- NSTextInsertionIndicator
- NSTextView
- NSTokenField
- NSTokenFieldCell
- NSView
- NSVisualEffectView
- NSWindow

## See Also

### AppKit Elements

struct NSAccessibility

A namespace for accessibility symbols for AppKit apps.

