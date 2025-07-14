

- Core Foundation
-  CFXMLParserOptions 

Structure

# CFXMLParserOptions

Options you can use to control the parser’s treatment of an XML document.

macOS

``` source
struct CFXMLParserOptions
```

## Overview

These are the various options you use to configure the parser. An option flag of 0 (kCFXMLParserNoOptions) leaves the XML as “intact” as possible (reports all structures; performs no replacements). Hence, to make the parser do the most work, returning only the pure element tree, set the option flag to allOptions.

## Topics

### Constants

static var validateDocument: CFXMLParserOptions

Validates the document against its grammar from the DTD, reporting any errors. Currently not supported.

static var skipMetaData: CFXMLParserOptions

Silently skip over metadata constructs (the DTD and comments).

static var replacePhysicalEntities: CFXMLParserOptions

Replaces declared entities like `&lt`;. Note that other than the 5 predefined entities (`lt`, `gt`, `quot`, `amp`, `apos`), these must be defined in the DTD. Currently not supported.

static var skipWhitespace: CFXMLParserOptions

static var resolveExternalEntities: CFXMLParserOptions

Resolves all external entities.

static var addImpliedAttributes: CFXMLParserOptions

Where the DTD specifies implied attribute-value pairs for a particular element, add those pairs to any occurrences of the element in the element tree. Currently not supported.

static var allOptions: CFXMLParserOptions

Makes the parser do the most work, returning only the pure elementtree.

### Initializers

init(rawValue: CFOptionFlags)

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

### Constants

struct CFXMLParserStatusCode

The various status and error flags that can be returned by the parser.

