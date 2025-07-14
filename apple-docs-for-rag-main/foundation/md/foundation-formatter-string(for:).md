

- Foundation
- Formatter
-  string(for:) 

Instance Method

# string(for:)

The default implementation of this method raises an exception.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(for obj: Any?) -> String?
```

## Parameters 

`obj`  

The object for which a textual representation is returned.

## Return Value

An `NSString` object that textually represents `object` for display. Returns `nil` if `object` is not of the correct class.

## Discussion

When implementing a subclass, return the `NSString` object that textually represents the cell’s object for display and—if editingString(for:) is unimplemented—for editing. First test the passed-in object to see if it’s of the correct class. If it isn’t, return `nil`; but if it is of the right class, return a properly formatted and, if necessary, localized string. (See the specification of the NSString class for formatting and localizing details.)

The following implementation (which is paired with the getObjectValue(_:for:errorDescription:) example above) prefixes a two-digit float representation with a dollar sign:

```
- (NSString *)stringForObjectValue:(id)anObject {

    if (![anObject isKindOfClass:[NSNumber class]]) {
        return nil;
    }
    return [NSString stringWithFormat:@"$%.2f", [anObject  floatValue]];
}
```

## See Also

### Related Documentation

Data Formatting Guide

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

The default implementation of this method raises an exception.

### Getting Textual Representations of Object Values

func attributedString(for: Any, withDefaultAttributes: [NSAttributedString.Key : Any]?) -> NSAttributedString?

The default implementation returns `nil` to indicate that the formatter object does not provide an attributed string.

func editingString(for: Any) -> String?

The default implementation of this method invokes string(for:).

