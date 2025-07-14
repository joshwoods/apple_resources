

- XCUIAutomation
- XCUIElementQuery
-  element(matching:) 

Instance Method

# element(matching:)

Matches the predicate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func element(matching predicate: NSPredicate) -> XCUIElement
```

## Parameters 

`predicate`  

The predicate to match.

## Discussion

The predicate evaluates against objects that conform to the XCUIElementAttributes protocol.

Note

Where possible, use NSExpression-based or format-string-based predicates with this method in preference to block-based predicates. This enables the framework to optimize the query’s performance.

## See Also

### Accessing matched elements

var allElementsBoundByAccessibilityElement: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound to the resulting accessibility elements.

var allElementsBoundByIndex: [XCUIElement]

Immediately evaluates the query and returns an array of elements bound by the index of each result.

var count: Int

Evaluates the query and returns the number of elements that match.

var element: XCUIElement

The query’s single matching element.

func element(boundBy: Int) -> XCUIElement

Uses an index into the query’s results to determine which underlying accessibility element to use.

func element(matching: XCUIElement.ElementType, identifier: String?) -> XCUIElement

Matches the provided element type and identifier.

subscript(String) -> XCUIElement

Returns a descendant element that matches a provided identifier.

func element(at: Int) -> XCUIElement

Returns an element that resolves to the index into the query’s result set.

Deprecated

