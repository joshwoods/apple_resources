

- Core Services
-  Dictionary Services 

API Collection

# Dictionary Services

Look for words and phrases in system dictionaries.

## Topics

### Functions

func DCSGetTermRangeInString(DCSDictionary?, CFString, CFIndex) -> CFRange

Determines the range of the longest word or phrase with respect to an offset.

func DCSCopyTextDefinition(DCSDictionary?, CFString, CFRange) -> Unmanaged&lt;CFString>?

Returns the definition associated with the provided text range.

### Data Types

class DCSDictionary

An opaque object that represents a dictionary file.

