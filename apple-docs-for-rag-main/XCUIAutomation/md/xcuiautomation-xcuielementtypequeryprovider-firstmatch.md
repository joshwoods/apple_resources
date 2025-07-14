

- XCUIAutomation
- XCUIElementTypeQueryProvider
-  firstMatch 

Instance Property

# firstMatch

The first element that matches the query.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var firstMatch: XCUIElement { get }
```

**Required**

## Discussion

Use the firstMatch property when you know that there can only be one possible match for an element query. When you call firstMatch, the framework stops traversing your app’s accessibility hierarchy as soon as it finds a matching element, speeding up element query resolution.

Note

Only use firstMatch in cases where you know categorically that a single element matches a query. Accessing the firstMatch property doesn’t check for multiple conflicting matches in ambiguous cases. Use XCUIElementQuery‘s element property instead if you want to check for multiple matches before using the element, and to fail the test if there isn’t a single unique match.

## See Also

### Related Documentation

var element: XCUIElement

The query’s single matching element.

