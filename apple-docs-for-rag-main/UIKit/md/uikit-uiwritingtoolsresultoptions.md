

- UIKit
-  UIWritingToolsResultOptions 

Structure

# UIWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
struct UIWritingToolsResultOptions
```

## Overview

When configuring a text view, specify what type of text input you want Writing Tools to deliver to your view. You can ask it to return plain text without any attributes, or you can ask it to apply relevant formatting attributes to the text. You can even encourage it to return items in a list or format them in a table.

## Topics

### Getting the output options

static var plainText: UIWritingToolsResultOptions

An option to allow only plain text without any attributes in the returned text.

static var richText: UIWritingToolsResultOptions

An option to include style attributes consistent with the RTF format in the returned text.

static var list: UIWritingToolsResultOptions

An option to allow list-style formatting in the returned text.

static var table: UIWritingToolsResultOptions

An option to allow tabular layout attributes in the returned text.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuration

Customizing Writing Tools behavior for UIKit views

Modify the behavior of Writing Tools in standard iOS text views, and adjust your app’s behavior while the feature is active.

enum UIWritingToolsBehavior

Constants that specify the writing tools experience for the underlying view.

