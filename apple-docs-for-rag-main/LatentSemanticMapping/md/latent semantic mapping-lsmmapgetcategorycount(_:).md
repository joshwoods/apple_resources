

- Latent Semantic Mapping
-  LSMMapGetCategoryCount(\_:) 

Function

# LSMMapGetCategoryCount(\_:)

Returns the number of categories in the map.

Mac CatalystmacOS

``` source
func LSMMapGetCategoryCount(_ mapref: LSMMap) -> CFIndex
```

## See Also

### Starting Training Mode

func LSMMapStartTraining(LSMMap) -> OSStatus

Puts the map into training mode, preparing it for the addition of more categories or texts.

func LSMMapAddCategory(LSMMap) -> LSMCategory

Adds another category and returns its category identifier.

func LSMMapSetStopWords(LSMMap, LSMText) -> OSStatus

Specifies which words to omit from all classification efforts.

func LSMMapAddText(LSMMap, LSMText, LSMCategory) -> OSStatus

Adds a training text to the specified category.

func LSMMapAddTextWithWeight(LSMMap, LSMText, LSMCategory, Float) -> OSStatus

Adds a training text to the specified category with a weight other than 1.

typealias LSMCategory

An integral type that represents a category.

