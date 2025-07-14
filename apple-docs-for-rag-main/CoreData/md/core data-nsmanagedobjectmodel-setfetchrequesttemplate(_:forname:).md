

- Core Data
- NSManagedObjectModel
-  setFetchRequestTemplate(\_:forName:) 

Instance Method

# setFetchRequestTemplate(\_:forName:)

Associates the specified fetch request with the receiver using the given name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setFetchRequestTemplate(
    _ fetchRequestTemplate: NSFetchRequest?,
    forName name: String
)
```

## Parameters 

`fetchRequestTemplate`  

A fetch request, typically containing predicates with variables for substitution.

`name`  

A string that specifies the name of the fetch request template.

## Discussion

For more details on using this method, see Creating Predicates.

### Special Considerations

This method raises an exception if the receiver has been used by an object graph manager.

## See Also

### Manipulating fetch request templates

var fetchRequestTemplatesByName: [String : NSFetchRequest&lt;any NSFetchRequestResult>]

A dictionary of the receiver’s fetch request templates, keyed by name.

func fetchRequestTemplate(forName: String) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns the fetch request with a specified name.

func fetchRequestFromTemplate(withName: String, substitutionVariables: [String : Any]) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns a copy of the fetch request template with the variables substituted by values from the substitutions dictionary.

