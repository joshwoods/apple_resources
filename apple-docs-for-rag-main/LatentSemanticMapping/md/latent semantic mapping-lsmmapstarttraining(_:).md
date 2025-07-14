

- Latent Semantic Mapping
-  LSMMapStartTraining(\_:) 

Function

# LSMMapStartTraining(\_:)

Puts the map into training mode, preparing it for the addition of more categories or texts.

Mac CatalystmacOS

``` source
func LSMMapStartTraining(_ mapref: LSMMap) -> OSStatus
```

## Discussion

This function is somewhat computationally expensive, as it requires substantial data structure reorganization.

## See Also

### Starting Training Mode

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

