

- XCUIAutomation
- XCUIElementQuery
-  element 

Instance Property

# element

The query’s single matching element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var element: XCUIElement { get }
```

## Discussion

Use the element property to access a query’s result when you expect a single matching element for the query, but want to check for multiple ambiguous matches before accessing the result. The element property traverses your app’s accessibility tree to check for multiple matching elements before returning, and fails the current test if there isn’t a single matching element.

In cases where you know categorically that there’s a single matching element, use the XCUIElementTypeQueryProvider firstMatch property instead. The firstMatch property stops traversing your app’s accessibility hierarchy as soon as it finds a matching element, speeding up element query resolution.

## See Also

### Related Documentation

var firstMatch: XCUIElement

The first element that matches the query.

**Required**

### Accessing matched elements

var allElementsBoundByAccessibilityElement: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound to the resulting accessibility elements.

var allElementsBoundByIndex: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound by the index of each result.

var count: Int

Evaluates the query and returns the number of elements that match.

func element(boundBy: Int) -> XCUIElement

Uses an index into the query’s results to determine which underlying accessibility element to use.

func element(matching: NSPredicate) -> XCUIElement

Matches the predicate.

func element(matching: XCUIElement.ElementType, identifier: String?) -> XCUIElement

Matches the provided element type and identifier.

subscript(String) -> XCUIElement

Returns a descendant element that matches a provided identifier.

func element(at: Int) -> XCUIElement

Returns an element that resolves to the index into the query’s result set.

Deprecated

