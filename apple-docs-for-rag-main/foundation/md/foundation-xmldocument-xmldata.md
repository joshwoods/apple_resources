

- Foundation
- XMLDocument
-  xmlData 

Instance Property

# xmlData

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var xmlData: Data { get }
```

## Discussion

This method invokes xmlData(options:) with an option of `NSXMLNodeOptionsNone`. The encoding used is based on the value returned from characterEncoding or UTF-8 if no valid encoding is returned by that method.

## See Also

### Writing a Document as XML Data

func xmlData(options: XMLNode.Options) -> Data

Returns the XML string representation of the receiver—that is, the entire document—encapsulated in a data object.

