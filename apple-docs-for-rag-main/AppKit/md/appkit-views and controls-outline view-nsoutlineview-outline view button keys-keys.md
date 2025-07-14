

- AppKit
- Views and Controls
- Outline View
- NSOutlineView
-  Outline View Button Keys 

API Collection

# Outline View Button Keys

These keys are used by the outline view to create disclosure buttons that collapse and expand items.

## Overview

The outline view creates these buttons by calling its inherited makeView(withIdentifier:owner:) method, passing in the key as the identifier and the delegate as the owner.

Note

These keys are backwards compatible to OS X v10.7, however, the symbol is not exported prior to v10.9 and the string value (`@"NSOutlineViewDisclosureButtonKey"`) must be used.

## Topics

### Constants

class let disclosureButtonIdentifier: NSUserInterfaceItemIdentifier

The normal triangle disclosure button.

class let showHideButtonIdentifier: NSUserInterfaceItemIdentifier

The Show/Hide button.

## See Also

### Constants

Drop on Item Index

This constant defines an index that allows you to drop an item directly on a target.

