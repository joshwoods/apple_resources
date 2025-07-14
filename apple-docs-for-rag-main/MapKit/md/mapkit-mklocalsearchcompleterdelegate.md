

- MapKit
-  MKLocalSearchCompleterDelegate 

Protocol

# MKLocalSearchCompleterDelegate

Methods the delegate calls with search completion data.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
protocol MKLocalSearchCompleterDelegate : NSObjectProtocol
```

## Overview

You use this protocol when implementing an autocomplete solution for a map in your app. As the user types search terms, use an MKLocalSearchCompleter object to start searching for valid completions. The delegate you assign to that object needs to conform to this protocol. As it receives completions, the local search completer calls the methods of this protocol to deliver the results.

## Topics

### Getting the search results

func completerDidUpdateResults(MKLocalSearchCompleter)

Tells the method when the specified search completer updates its array of search completions.

func completer(MKLocalSearchCompleter, didFailWithError: any Error)

Tells the method when the specified search completer is unable to generate a list of search results.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving the search results

var delegate: (any MKLocalSearchCompleterDelegate)?

The object that receives the completion results.

