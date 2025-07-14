

- UIKit
-  UITextDirection 

Structure

# UITextDirection

The direction of the text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UITextDirection
```

## Overview

This parameter is used in methods declared by the UITextInputTokenizer protocol. This general direction type subsumes constants of the UITextStorageDirection and UITextLayoutDirection types.

## Topics

### Text direction types

static func layout(UITextLayoutDirection) -> UITextDirection

Specifies the direction of text layout.

static func storage(UITextStorageDirection) -> UITextDirection

Specifies the direction of text storage.

### Initializers

init(rawValue: Int)

Creates a text direction with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum UITextStorageDirection

The direction of text storage.

enum UITextLayoutDirection

The direction of text layout.

