

- Foundation
- PersonNameComponentsFormatter
-  getObjectValue(\_:for:errorDescription:) 

Instance Method

# getObjectValue(\_:for:errorDescription:)

Returns by reference a person name components object after creating it from a given string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getObjectValue(
    _ obj: AutoreleasingUnsafeMutablePointer?,
    for string: String,
    errorDescription error: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`obj`  

On return, contains an instance of NSPersonNameComponents, or `nil` if conversion failed.

`string`  

A string that is parsed to create a person name components object.

`error`  

If an error occurs, upon return contains an NSError object in the NSCocoaErrorDomain with code NSFormattingError that explains why the conversion failed. If you pass in `nil` for error, you are indicating that you are not interested in error information.

## Return Value

true if conversion succeeded; otherwise false.

## See Also

### Converting Between Person Name Components and Strings

class func localizedString(from: PersonNameComponents, style: PersonNameComponentsFormatter.Style, options: PersonNameComponentsFormatter.Options) -> String

Returns a string formatted for a given `NSPersonNameComponents` object using the provided style and options.

func string(from: PersonNameComponents) -> String

Returns a string formatted for a given `NSPersonNameComponents` object.

func annotatedString(from: PersonNameComponents) -> NSAttributedString

Returns an attributed string formatted for a given `NSPersonNameComponents` object, with attribute annotations for each component.

func personNameComponents(from: String) -> PersonNameComponents?

Returns a person name components object from a given string.

