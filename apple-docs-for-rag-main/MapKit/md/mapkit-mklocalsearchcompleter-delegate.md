

- MapKit
- MKLocalSearchCompleter
-  delegate 

Instance Property

# delegate

The object that receives the completion results.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
weak var delegate: (any MKLocalSearchCompleterDelegate)? { get set }
```

## Discussion

You must provide a delegate object to receive completion results and to handle any errors that might occur. For more information about the methods of the delegate protocol, see MKLocalSearchCompleterDelegate.

## See Also

### Receiving the search results

protocol MKLocalSearchCompleterDelegate

Methods the delegate calls with search completion data.

