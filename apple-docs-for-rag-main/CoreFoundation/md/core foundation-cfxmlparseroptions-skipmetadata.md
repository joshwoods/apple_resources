

- Core Foundation
- CFXMLParserOptions
-  skipMetaData 

Type Property

# skipMetaData

Silently skip over metadata constructs (the DTD and comments).

macOS

``` source
static var skipMetaData: CFXMLParserOptions { get }
```

## See Also

### Constants

static var validateDocument: CFXMLParserOptions

Validates the document against its grammar from the DTD, reporting any errors. Currently not supported.

static var replacePhysicalEntities: CFXMLParserOptions

Replaces declared entities like `&lt`;. Note that other than the 5 predefined entities (`lt`, `gt`, `quot`, `amp`, `apos`), these must be defined in the DTD. Currently not supported.

static var skipWhitespace: CFXMLParserOptions

static var resolveExternalEntities: CFXMLParserOptions

Resolves all external entities.

static var addImpliedAttributes: CFXMLParserOptions

Where the DTD specifies implied attribute-value pairs for a particular element, add those pairs to any occurrences of the element in the element tree. Currently not supported.

static var allOptions: CFXMLParserOptions

Makes the parser do the most work, returning only the pure elementtree.

