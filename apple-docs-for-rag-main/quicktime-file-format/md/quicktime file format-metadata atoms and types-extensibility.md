

- QuickTime File Format
- Metadata atoms and types
-  Extensibility 

Article

# Extensibility

Avoid issues building extensibility into your file.

## Overview

In order to allow metadata to be rewritten easily and without the need to rewrite the entire QuickTime movie file, free space atoms may occur anywhere in the definition of the metadata atom between the positions of other atoms contained by the metadata atom. Free space atoms may not be inserted between items in the metadata item list atom or within atoms in the metadata item list atom. This restriction on free space atom definition avoids the risk of confusing a free space atom with a meaning of a `‘free’` identifier or a value atom of type `‘free’` defined in the context of the metadata atom structure.

Similarly, UUID atoms for specific extensions may be placed in any position where a succession of atoms is permitted. Note that UUID atoms should not be created for atoms already defined using four-character codes.

Unrecognized atoms (that is, those atoms whose types not defined in the context of the metadata atom structure and are contained within the metadata item list atom) are ignored.

## See Also

### Types and usage

Localization list sets

Provide metadata for more than one country or language.

Type indicator

Four bytes that indicate a type of data that QuickTime supports.

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

