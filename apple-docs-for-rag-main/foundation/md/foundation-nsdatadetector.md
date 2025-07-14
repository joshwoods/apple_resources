

- Foundation
-  NSDataDetector 

Class

# NSDataDetector

A specialized regular expression object that matches natural language text for predefined data patterns.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDataDetector
```

## Overview

Find dates, addresses, links, phone numbers, and transit information in natural language text with `NSDataDetector`.

`NSDataDetector` returns the results of matching content in NSTextCheckingResult objects. The NSTextCheckingResult objects that `NSDataDetector` returns are different from those that NSRegularExpression returns. The results are one of the data detector’s types and contain the corresponding properties. For example, results of type date have a date, timeZone, and duration; and results of type link have a url.

Important

Don’t use `NSDataDetector` to validate data. `NSDataDetector` discards potential matches in case of uncertainty. Use a class specific to the type of data for validation instead. For example, attempt to instantiate a URL object using init(string:) to validate a URL string. A valid URL string returns an instance of URL, while an invalid URL string returns nil.

### Examples

The following shows several graduated examples of using the `NSDataDetector` class.

This code fragment creates a data detector that finds URL links and phone numbers. If an error occurs, it returns in `error`.

```
   NSError *error = nil;
   NSDataDetector *detector = [NSDataDetector dataDetectorWithTypes:NSTextCheckingTypeLink|NSTextCheckingTypePhoneNumber
                                                              error:&error];
```

After creating the data detector instance, you can determine the number of matches within a range of a string using the `NSRegularExpression` method numberOfMatches(in:options:range:).

```
   NSUInteger numberOfMatches = [detector numberOfMatchesInString:string
                                                          options:0
                                                            range:NSMakeRange(0, [string length])];
```

If you’re interested only in the overall range of the first match, the numberOfMatches(in:options:range:) method provides it. However, with data detectors, this is less likely than with regular expressions because clients are usually interested in additional information as well.

The additional information available depends on the type of the result. For results of type link, it’s the `URL` property that’s significant. For results of type `NSTextCheckingTypePhoneNumber` , it’s the `phoneNumber` property instead.

The matches(in:options:range:) method is similar to firstMatch(in:options:range:), except that it returns all matches rather than only the first. The following code fragment finds all the matches for links and phone numbers in a string:

```
   NSArray *matches = [detector matchesInString:string
                                        options:0
                                          range:NSMakeRange(0, [string length])];
   for (NSTextCheckingResult *match in matches) {
        NSRange matchRange = [match range];
        if ([match resultType] == NSTextCheckingTypeLink) {
            NSURL *url = [match URL];
        } else if ([match resultType] == NSTextCheckingTypePhoneNumber) {
            NSString *phoneNumber = [match phoneNumber];
        }
   }
```

The `NSRegularExpression` block object enumerator is the most general and flexible of the matching methods. It allows you to iterate through matches in a string, performing arbitrary actions on each as specified by the code in the block, and to stop partway through if desired. In the following code fragment, the iteration stops after finding a certain number of matches:

```
   __block NSUInteger count = 0;
   [detector enumerateMatchesInString:string
                              options:0
                                range:NSMakeRange(0, [string length])
                           usingBlock:^(NSTextCheckingResult *match, NSMatchingFlags flags, BOOL *stop){
        NSRange matchRange = [match range];
        if ([match resultType] == NSTextCheckingTypeLink) {
            NSURL *url = [match URL];
        } else if ([match resultType] == NSTextCheckingTypePhoneNumber) {
            NSString *phoneNumber = [match phoneNumber];
        }
        if (++count >= 100) *stop = YES;
   }];
```

Note

Only use `NSDataDetector` on natural language text.

If you expect text to be in a particular format, use an Formatter or ValueTransformer subclass instead. For instance, if you’re expecting a date field to be an ISO 8601 timestamp, use DateFormatter to parse that into an NSDate object.

If the text is in a machine-readable format, such as XML or JSON, extract the natural language text, such as by using XMLParser or JSONSerialization, and match on that rather than attempt to match on the entire document.

## Topics

### Creating data detector instances

init(types: NSTextCheckingTypes) throws

Initializes and returns a data detector instance.

### Getting the checking types

var checkingTypes: NSTextCheckingTypes

Returns the checking types for the data detector.

## Relationships

### Inherits From

- NSRegularExpression

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Pattern Matching

class Scanner

A string parser that scans for substrings or characters in a character set, and for numeric values from decimal, hexadecimal, and floating-point representations.

class NSRegularExpression

An immutable representation of a compiled regular expression that you apply to Unicode strings.

class NSTextCheckingResult

An occurrence of textual content found during the analysis of a block of text, such as when matching a regular expression.

let NSNotFound: Int

A value indicating that a requested item couldn’t be found or doesn’t exist.

