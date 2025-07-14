

- Core Data
- NSManagedObjectModel
-  fetchRequestTemplatesByName 

Instance Property

# fetchRequestTemplatesByName

A dictionary of the receiver’s fetch request templates, keyed by name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchRequestTemplatesByName: [String : NSFetchRequest] { get }
```

## Discussion

If the template contains a predicate with substitution variables, you should instead use fetchRequestFromTemplate(withName:substitutionVariables:) to create a new fetch request.

## See Also

### Manipulating fetch request templates

func fetchRequestTemplate(forName: String) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns the fetch request with a specified name.

func fetchRequestFromTemplate(withName: String, substitutionVariables: [String : Any]) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns a copy of the fetch request template with the variables substituted by values from the substitutions dictionary.

func setFetchRequestTemplate(NSFetchRequest&lt;any NSFetchRequestResult>?, forName: String)

Associates the specified fetch request with the receiver using the given name.

