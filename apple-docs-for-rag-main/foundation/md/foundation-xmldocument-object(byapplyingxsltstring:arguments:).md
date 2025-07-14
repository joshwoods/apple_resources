

- Foundation
- XMLDocument
-  object(byApplyingXSLTString:arguments:) 

Instance Method

# object(byApplyingXSLTString:arguments:)

Applies the XSLT pattern rules and templates (specified as a string) to the receiver and returns a document object containing transformed XML or HTML markup.

Mac Catalyst 13.0+macOS 10.0+

``` source
func object(
    byApplyingXSLTString xslt: String,
    arguments: [String : String]?
) throws -> Any
```

## Parameters 

`xslt`  

A string object containing the XSLT pattern rules and templates.

`arguments`  

A dictionary containing NSString key-value pairs that are passed as runtime parameters to the XSLT processor. Pass in `nil` if you have no parameters to pass.

Note

Several XML websites discuss XSLT parameters, including O’Reilly Media’s http://www.xml.com.

## Return Value

Depending on intended output, the method returns an `NSXMLDocument` object *or* an NSData data containing transformed XML or HTML markup. If the message is supposed to create plain text or RTF, then an `NSData` object is returned, otherwise an XML document object. The method returns `nil` if XSLT processing did not succeed.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Transforming a Document Using XSLT

func object(byApplyingXSLT: Data, arguments: [String : String]?) throws -> Any

Applies the XSLT pattern rules and templates (specified as a data object) to the receiver and returns a document object containing transformed XML or HTML markup.

func objectByApplyingXSLT(at: URL, arguments: [String : String]?) throws -> Any

Applies the XSLT pattern rules and templates located at a specified URL to the receiver and returns a document object containing transformed XML markup or an NSData object containing plain text, RTF text, and so on.

