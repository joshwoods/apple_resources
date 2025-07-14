

- MapKit
- MKLocalSearchCompleter
-  queryFragment 

Instance Property

# queryFragment

The search string that you want completions for.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
var queryFragment: String { get set }
```

## Discussion

Assigning a string to this property initiates a search based on that string. The completer object waits a short amount of time before initiating new searches. This delay gives you enough time to update the search string based on typed input from the user. For example, if you’re using a text field to manage the input from the user, use the textField(_:shouldChangeCharactersIn:replacementString:) method of the text field’s delegate to update the value of this property, as the following example shows:

```
- (BOOL)textField:(UITextField *)textField shouldChangeCharactersInRange:(NSRange)range
         replacementString:(NSString *)string {
    self.completer.queryFragment = textField.text;

    return YES;
}
```

## See Also

### Specifying the query attributes

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var region: MKCoordinateRegion

The region that defines the geographic scope of the search.

var regionPriority: MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

var resultTypes: MKLocalSearchCompleter.ResultType

The types of search completions to include.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point of interest categories to include or exclude in the search.

var filterType: MKLocalSearchCompleter.FilterType

The filter options for the search results.

Deprecated

enum FilterType

Constants indicating the types of search completions to return.

Deprecated

struct ResultType

Options that indicate types of search completions.

