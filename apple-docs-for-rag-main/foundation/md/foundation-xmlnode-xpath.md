

- Foundation
- XMLNode
-  xPath 

Instance Property

# xPath

Returns the XPath expression identifying the receiver’s location in the document tree.

Mac Catalyst 13.0+macOS 10.0+

``` source
var xPath: String? { get }
```

## Discussion

For example, this method might return a string such as “foo/bar\[2\]/baz”. The result of this method can be used directly in the nodes(forXPath:) and objects(forXQuery:constants:) methods.

## See Also

### Executing Queries

func nodes(forXPath: String) throws -> [XMLNode]

Returns the nodes resulting from executing an XPath query upon the receiver.

func objects(forXQuery: String) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

func objects(forXQuery: String, constants: [String : Any]?) throws -> [Any]

Returns the objects resulting from executing an XQuery query upon the receiver.

