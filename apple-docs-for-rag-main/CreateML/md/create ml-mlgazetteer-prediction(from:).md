

- Create ML
- MLGazetteer
-  prediction(from:) 

Instance Method

# prediction(from:)

Predicts the label for the given term.

macOS 10.15+

``` source
func prediction(from text: String) throws -> String
```

## Parameters 

`text`  

The input term.

## Return Value

A label.

## See Also

### Testing a gazetteer

func predictions(from: [String]) throws -> [String]

Predicts the labels for the given terms.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Predicts the labels for the given terms in the table column.

Deprecated

