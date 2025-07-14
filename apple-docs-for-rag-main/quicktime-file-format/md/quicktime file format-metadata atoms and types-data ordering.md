

- QuickTime File Format
- Metadata atoms and types
-  Data ordering 

Article

# Data ordering

Represent multiple representations of the same information, differing either by language or storage type or by the size or nature of the data.

## Overview

Multiple values for the same tag represent multiple representations of the same information, differing either by language or storage type or by the size or nature of the data. For example, an artist name may be supplied in three ways:

- as a large JPEG of their signature

- as a smaller ‘thumbnail’ JPEG of their signature

- as text

An application may then choose the variation of the the artist name to display based on the size it needs.

Data must be ordered in each item from the most-specific data to the most general. An application may, if it wishes, stop ‘searching’ for a value once it finds a value that it can display (it has an acceptable locale and type).

## See Also

### Types and usage

Extensibility

Avoid issues building extensibility into your file.

Localization list sets

Provide metadata for more than one country or language.

Type indicator

Four bytes that indicate a type of data that QuickTime supports.

Locale indicator

A four-byte value that indicates a locale.

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

