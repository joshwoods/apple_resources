

- UIKit
- NSTextLayoutFragment
-  NSTextLayoutFragment.EnumerationOptions 

Structure

# NSTextLayoutFragment.EnumerationOptions

Values that describe options for enumerating text layout fragments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
struct EnumerationOptions
```

## Topics

### Creating a layout fragment enumeration

init(rawValue: UInt)

Creates an instance of the enumeration with the provided unsigned integer value.

### Layout fragment characteristics

static var ensuresExtraLineFragment: NSTextLayoutFragment.EnumerationOptions

Synthesize the extra line fragment when necessary.

static var ensuresLayout: NSTextLayoutFragment.EnumerationOptions

When enumerating, tell the layout fragments to layout their contents.

static var estimatesSize: NSTextLayoutFragment.EnumerationOptions

When enumerating, tell the layout fragments to estimate their size.

static var reverse: NSTextLayoutFragment.EnumerationOptions

Causes the enumeration to start from the last element.

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

### Accessing and updating the text

func enumerateTextElements(from: (any NSTextLocation)?, options: NSTextContentManager.EnumerationOptions, using: (NSTextElement) -> Bool) -> (any NSTextLocation)?

Enumerates text elements starting at the text location you provide.

**Required**

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location from location with offset you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement]?)

Replaces the characters specified by range with the text elements you provide.

**Required**

