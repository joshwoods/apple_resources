

- QuickTime File Format
- Metadata atoms and types
-  Type indicator 

Article

# Type indicator

Four bytes that indicate a type of data that QuickTime supports.

## Overview

The type indicator is formed of four bytes split between two fields. The first byte indicates the set of types from which the type is drawn. The second through fourth byte forms the second field and its interpretation depends upon the value in the first field.

The indicator byte must have a value of `0`, meaning the type is drawn from the well-known set of types. All other values are reserved.

If the type indicator byte is `0`, the following 24 bits hold the well-known type. Please refer to the list of Well-known types.

## See Also

### Types and usage

Extensibility

Avoid issues building extensibility into your file.

Localization list sets

Provide metadata for more than one country or language.

Locale indicator

A four-byte value that indicates a locale.

Data ordering

Represent multiple representations of the same information, differing either by language or storage type or by the size or nature of the data.

Well-known types

Basic data types.

Location metadata

Storing the location coordinates, as well as several auxiliary pieces of information about a location, as metadata.

QuickTime metadata keys

Use QuickTime keys to hold data in a Metadata atom.

Direction definition

Define a direction in metadata keys.

Metadata handling

Handling metadata in other file formats.

