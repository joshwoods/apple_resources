

- XCUIAutomation
- XCUIElementQuery
-  element(matching:identifier:) 

Instance Method

# element(matching:identifier:)

Matches the provided element type and identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func element(
    matching elementType: XCUIElement.ElementType,
    identifier: String?
) -> XCUIElement
```

## Parameters 

`elementType`  

The element type to match.

`identifier`  

An optional identifier string to match against any one of each element’s identifying properties: identifier, title, label, value, or placeholderValue.

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

func element(matching: NSPredicate) -> XCUIElement

Matches the predicate.

subscript(String) -> XCUIElement

Returns a descendant element that matches a provided identifier.

func element(at: Int) -> XCUIElement

Returns an element that resolves to the index into the query’s result set.

Deprecated

