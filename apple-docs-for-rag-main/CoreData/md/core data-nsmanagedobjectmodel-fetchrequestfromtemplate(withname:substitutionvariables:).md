

- Core Data
- NSManagedObjectModel
-  fetchRequestFromTemplate(withName:substitutionVariables:) 

Instance Method

# fetchRequestFromTemplate(withName:substitutionVariables:)

Returns a copy of the fetch request template with the variables substituted by values from the substitutions dictionary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func fetchRequestFromTemplate(
    withName name: String,
    substitutionVariables variables: [String : Any]
) -> NSFetchRequest?
```

## Parameters 

`name`  

A string containing the name of a fetch request template.

`variables`  

A dictionary containing key-value pairs where the keys are the names of variables specified in the template; the corresponding values are substituted before the fetch request is returned. The dictionary must provide values for all the variables in the template.

## Return Value

A copy of the fetch request template with the variables substituted by values from `variables`.

## Discussion

The `variables` dictionary must provide values for all the variables. If you want to test for a nil value, use `[NSNull null]`.

This method provides the usual way to bind an “abstractly” defined fetch request template to a concrete fetch. For more details on using this method, see Creating Predicates.

## See Also

### Manipulating fetch request templates

var fetchRequestTemplatesByName: [String : NSFetchRequest&lt;any NSFetchRequestResult>]

A dictionary of the receiver’s fetch request templates, keyed by name.

func fetchRequestTemplate(forName: String) -> NSFetchRequest&lt;any NSFetchRequestResult>?

Returns the fetch request with a specified name.

func setFetchRequestTemplate(NSFetchRequest&lt;any NSFetchRequestResult>?, forName: String)

Associates the specified fetch request with the receiver using the given name.

