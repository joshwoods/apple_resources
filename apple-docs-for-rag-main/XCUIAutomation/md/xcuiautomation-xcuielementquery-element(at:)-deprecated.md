

- XCUIAutomation
- XCUIElementQuery
-  element(at:) Deprecated

Instance Method

# element(at:)

Returns an element that resolves to the index into the query’s result set.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+tvOS

``` source
@MainActor
func element(at index: Int) -> XCUIElement
```

Deprecated

Use element(boundBy:) instead.

## Parameters 

`index`  

The element index to use.

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

func element(matching: XCUIElement.ElementType, identifier: String?) -> XCUIElement

Matches the provided element type and identifier.

subscript(String) -> XCUIElement

Returns a descendant element that matches a provided identifier.

