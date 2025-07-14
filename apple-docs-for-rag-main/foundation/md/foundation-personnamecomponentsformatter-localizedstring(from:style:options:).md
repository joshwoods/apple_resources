

- Foundation
- PersonNameComponentsFormatter
-  localizedString(from:style:options:) 

Type Method

# localizedString(from:style:options:)

Returns a string formatted for a given `NSPersonNameComponents` object using the provided style and options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localizedString(
    from components: PersonNameComponents,
    style nameFormatStyle: PersonNameComponentsFormatter.Style,
    options nameOptions: PersonNameComponentsFormatter.Options = []
) -> String
```

## Parameters 

`components`  

The name components to be formatted.

`nameFormatStyle`  

A format style for the name components. For possible values, see PersonNameComponentsFormatter.Style.

`nameOptions`  

The formatting options for the name components. For possible values, see PersonNameComponentsFormatter.Options.

## Return Value

A formatted string representation of the given name components.

## Discussion

This method is a convenience for formatting name components without creating an instance of `NSPersonNameComponentsFormatter`. For greater customizability, you can create an instance of `NSPersonNameComponentsFormatter` and use string(from:) instead.

## See Also

### Converting Between Person Name Components and Strings

func string(from: PersonNameComponents) -> String

Returns a string formatted for a given `NSPersonNameComponents` object.

func annotatedString(from: PersonNameComponents) -> NSAttributedString

Returns an attributed string formatted for a given `NSPersonNameComponents` object, with attribute annotations for each component.

func personNameComponents(from: String) -> PersonNameComponents?

Returns a person name components object from a given string.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

Returns by reference a person name components object after creating it from a given string.

