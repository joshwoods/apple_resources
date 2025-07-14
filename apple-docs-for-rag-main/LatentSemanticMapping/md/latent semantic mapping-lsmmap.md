

- Latent Semantic Mapping
-  LSMMap 

Class

# LSMMap

A map between a set of categories and related text.

Mac CatalystmacOS

``` source
class LSMMap
```

## Overview

An LSMMap is a mutable, opaque Core Foundation type that represents a map.

## Topics

### Creating a Map

func LSMMapCreate(CFAllocator?, CFOptionFlags) -> Unmanaged&lt;LSMMap>

Creates a new Latent Semantic Mapping map.

Map Flags

Options for creating a map.

### Managing a Map’s Properties

func LSMMapSetProperties(LSMMap, CFDictionary)

Sets a dictionary of properties for the map.

func LSMMapGetProperties(LSMMap) -> Unmanaged&lt;CFDictionary>

Gets a dictionary of properties for the map.

Map Properties

Special properties that determine a map’s behavior.

### Starting Training Mode

func LSMMapStartTraining(LSMMap) -> OSStatus

Puts the map into training mode, preparing it for the addition of more categories or texts.

func LSMMapAddCategory(LSMMap) -> LSMCategory

Adds another category and returns its category identifier.

func LSMMapGetCategoryCount(LSMMap) -> CFIndex

Returns the number of categories in the map.

func LSMMapSetStopWords(LSMMap, LSMText) -> OSStatus

Specifies which words to omit from all classification efforts.

func LSMMapAddText(LSMMap, LSMText, LSMCategory) -> OSStatus

Adds a training text to the specified category.

func LSMMapAddTextWithWeight(LSMMap, LSMText, LSMCategory, Float) -> OSStatus

Adds a training text to the specified category with a weight other than 1.

typealias LSMCategory

An integral type that represents a category.

### Starting Classification Mode

func LSMMapCompile(LSMMap) -> OSStatus

Compiles the map into executable form and puts it into mapping mode, preparing it for the classification of texts.

func LSMMapCreateClusters(CFAllocator?, LSMMap, CFArray?, CFIndex, CFOptionFlags) -> Unmanaged&lt;CFArray>?

Computes a set of clusters that group similar categories or words.

Clustering Flags

Options for creating clusters.

func LSMMapApplyClusters(LSMMap, CFArray) -> OSStatus

Groups categories or words (tokens) into the specified sets of clusters.

### Loading and Saving a Map

func LSMMapCreateFromURL(CFAllocator?, CFURL, CFOptionFlags) -> Unmanaged&lt;LSMMap>?

Loads a map from the specified file.

func LSMMapWriteToURL(LSMMap, CFURL, CFOptionFlags) -> OSStatus

Compiles the map, if necessary, and stores it into the specified file.

func LSMMapWriteToStream(LSMMap, LSMText?, CFWriteStream, CFOptionFlags) -> OSStatus

Writes information about a map or text to a stream in text form.

Storage Flags

Options for loading and saving a map to a file.

### Getting the Type Identifier

func LSMMapGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for Latent Semantic Mapping maps.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Text Classification

class LSMText

An input text.

class LSMResult

A result of a lookup in a map.

