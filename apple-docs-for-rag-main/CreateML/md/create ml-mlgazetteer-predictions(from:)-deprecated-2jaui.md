

- Create ML
- MLGazetteer
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Predicts the labels for the given terms in the table column.

macOS 10.15–14.0Deprecated

``` source
func predictions(from texts: MLDataColumn) throws -> MLDataColumn
```

## Parameters 

`texts`  

The column of terms.

## Return Value

A column of labels.

## See Also

### Testing a gazetteer

func prediction(from: String) throws -> String

Predicts the label for the given term.

func predictions(from: [String]) throws -> [String]

Predicts the labels for the given terms.

