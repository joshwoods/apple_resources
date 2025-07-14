

- UIKit
- UIPasteboard
-  UIPasteboard.OptionsKey 

Structure

# UIPasteboard.OptionsKey

Options for describing pasteboard privacy.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct OptionsKey
```

## Overview

Use these options with the setItems(_:options:) method. Options that you set apply to all the items on a pasteboard.

## Topics

### Constants

static let expirationDate: UIPasteboard.OptionsKey

The time and date that you want the system to remove the pasteboard items from the pasteboard.

static let localOnly: UIPasteboard.OptionsKey

A Boolean value that specifies that the pasteboard items should not be available to other devices through the Handoff feature.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct Name

Constants that identify the name of a pasteboard.

Pasteboard Names

Names identifying the system pasteboards.

Pasteboard Data Type Representations

Pasteboard-item representation types, as for a given object value.

UserInfo Dictionary Keys

Use these keys to access the representation types of pasteboard items that you add to, or remove from, a pasteboard.

