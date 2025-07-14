

- Latent Semantic Mapping
-  LSMCategory 

Type Alias

# LSMCategory

An integral type that represents a category.

Mac CatalystmacOS

``` source
typealias LSMCategory = UInt32
```

## See Also

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

