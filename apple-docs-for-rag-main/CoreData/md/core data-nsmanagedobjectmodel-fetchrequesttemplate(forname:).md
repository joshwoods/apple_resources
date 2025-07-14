

- Core Data
- NSManagedObjectModel
-  fetchRequestTemplate(forName:) 

Instance Method

# fetchRequestTemplate(forName:)

Returns the fetch request with a specified name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func fetchRequestTemplate(forName name: String) -> NSFetchRequest?
```

## Parameters 

`name`  

A string containing the name of a fetch request template.

## Return Value

The fetch request named `name`.

## Discussion

If the template contains substitution variables, you should instead use fetchRequestFromTemplate(withName:substitutionVariables:) to create a new fetch request.

## See Also

### Manipulating fetch request templates

var fetchRequestTemplatesByName: [String : NSFetchRequest&lt;any NSFetchRequestResult>]

A dictionary of the receiver’s fetch request templates, keyed by name.

func fetchRequestFromTemplate(withName: String, substitutionVariables: [String : Any]) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns a copy of the fetch request template with the variables substituted by values from the substitutions dictionary.

func setFetchRequestTemplate(NSFetchRequest&lt;any NSFetchRequestResult>?, forName: String)

Associates the specified fetch request with the receiver using the given name.

