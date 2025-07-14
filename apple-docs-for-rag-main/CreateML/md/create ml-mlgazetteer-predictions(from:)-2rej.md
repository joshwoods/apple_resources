

- Create ML
- MLGazetteer
-  predictions(from:) 

Instance Method

# predictions(from:)

Predicts the labels for the given terms.

macOS 10.15+

``` source
func predictions(from texts: [String]) throws -> [String]
```

## Parameters 

`texts`  

The array of input terms.

## Return Value

An array of labels.

## See Also

### Testing a gazetteer

func prediction(from: String) throws -> String

Predicts the label for the given term.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Predicts the labels for the given terms in the table column.

Deprecated

