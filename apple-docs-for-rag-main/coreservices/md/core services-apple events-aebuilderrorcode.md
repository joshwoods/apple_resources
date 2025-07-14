

- Core Services
- Apple Events
-  AEBuildErrorCode 

Type Alias

# AEBuildErrorCode

Represents syntax errors found by an Apple Event build routine.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEBuildErrorCode = UInt32
```

## Topics

### Constants

var aeBuildSyntaxNoErr: Int

No error.

var aeBuildSyntaxBadToken: Int

An illegal character was specified.

var aeBuildSyntaxBadEOF: Int

An unexpected end of format string was encountered.

var aeBuildSyntaxNoEOF: Int

There were unexpected characters beyond the end of the format string.

var aeBuildSyntaxBadNegative: Int

A minus sign “-” was not followed by digits.

var aeBuildSyntaxMissingQuote: Int

A string was not terminated by a closing quotation mark.

var aeBuildSyntaxBadHex: Int

A hex string contained characters other than hexadecimal digits.

var aeBuildSyntaxOddHex: Int

A hex string contained an odd number of digits.

var aeBuildSyntaxNoCloseHex: Int

A hex string was missing a “\$” or “»” character.

var aeBuildSyntaxUncoercedHex: Int

A hex string must be coerced to a type.

var aeBuildSyntaxNoCloseString: Int

A string was missing a closing quote.

var aeBuildSyntaxBadDesc: Int

An illegal descriptor was specified.

var aeBuildSyntaxBadData: Int

Bad data was found inside a variable argument list.

var aeBuildSyntaxNoCloseParen: Int

A data value was missing a closing parenthesis.

var aeBuildSyntaxNoCloseBracket: Int

A comma or closing bracket “\]” was expected.

var aeBuildSyntaxNoCloseBrace: Int

A comma or closing brace “}” was expected.

var aeBuildSyntaxNoKey: Int

A keyword was missing from a descriptor.

var aeBuildSyntaxNoColon: Int

In a descriptor, one of the keywords was not followed by a colon.

var aeBuildSyntaxCoercedList: Int

Cannot coerce a list.

var aeBuildSyntaxUncoercedDoubleAt: Int

You must coerce a “@@” substitution.

