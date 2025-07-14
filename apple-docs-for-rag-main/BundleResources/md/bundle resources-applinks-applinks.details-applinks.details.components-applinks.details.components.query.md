

- Bundle Resources
- applinks
- applinks.Details
- applinks.Details.Components
-  applinks.Details.Components.Query 

Object

# applinks.Details.Components.Query

A dictionary of names and values to match with query items in a URL.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
object applinks.Details.Components.Query
```

## Properties

`Any Key`

`string`

## Discussion

The keys in this dictionary are NSURLQueryItem names and the values are patterns to match with the specified key’s value. This example code shows how to use a dictionary object for pattern matching with a URL query component:

```
"?": { "productID": "12345" }
```

The above definition matches a URL query component that has a name of `productID` and a value of `12345`.

