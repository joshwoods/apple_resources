

- Core Foundation
- CFXMLParserOptions
-  skipWhitespace 

Type Property

# skipWhitespace

macOS

``` source
static var skipWhitespace: CFXMLParserOptions { get }
```

## Discussion

Skip over all whitespace that does not abut non-whitespace character data. In other words, given “`  blah `,” the whitespace between foo’s open tag and bar’s open tag would be suppressed, but the whitespace around `blah` would be preserved.

## See Also

### Constants

static var validateDocument: CFXMLParserOptions

Validates the document against its grammar from the DTD, reporting any errors. Currently not supported.

static var skipMetaData: CFXMLParserOptions

Silently skip over metadata constructs (the DTD and comments).

static var replacePhysicalEntities: CFXMLParserOptions

Replaces declared entities like `&lt`;. Note that other than the 5 predefined entities (`lt`, `gt`, `quot`, `amp`, `apos`), these must be defined in the DTD. Currently not supported.

static var resolveExternalEntities: CFXMLParserOptions

Resolves all external entities.

static var addImpliedAttributes: CFXMLParserOptions

Where the DTD specifies implied attribute-value pairs for a particular element, add those pairs to any occurrences of the element in the element tree. Currently not supported.

static var allOptions: CFXMLParserOptions

Makes the parser do the most work, returning only the pure elementtree.

