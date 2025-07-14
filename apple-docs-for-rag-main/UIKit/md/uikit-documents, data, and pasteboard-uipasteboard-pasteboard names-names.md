

- UIKit
- Documents, data, and pasteboard
- UIPasteboard
-  Pasteboard Names 

API Collection

# Pasteboard Names

Names identifying the system pasteboards.

## Overview

You can access the general system pasteboard by calling the class method init(name:create:), specifying the `UIPasteboardNameGeneral` constant as the first argument. You can alternatively access the general pasteboard by calling the general class method. The general system pasteboard is persistent across device restarts, app uninstalls, and app restores.

## Topics

### Constants

static let general: UIPasteboard.Name

The name identifying the general pasteboard, which you use for general copy-cut-paste operations.

let UIPasteboardNameFind: String

The Find pasteboard is unavailable starting in iOS 10. (The name identifying the Find pasteboard, which, prior to iOS 10, was used in search operations. In such operations, the most recent search string in the search bar was put in the Find pasteboard.)

Deprecated

## See Also

### Constants

struct Name

Constants that identify the name of a pasteboard.

struct OptionsKey

Options for describing pasteboard privacy.

Pasteboard Data Type Representations

Pasteboard-item representation types, as for a given object value.

UserInfo Dictionary Keys

Use these keys to access the representation types of pasteboard items that you add to, or remove from, a pasteboard.

