

- Swift Testing
- Trait
-  bug(\_:id:\_:) 

Type Method

# bug(\_:id:\_:)

Construct a bug to track with a test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func bug(
    _ url: String? = nil,
    id: some Numeric,
    _ title: Comment? = nil
) -> Self
```

Available when `Self` is `Bug`.

## Parameters 

`url`  

A URL referring to this bug in the associated bug-tracking system.

`id`  

The unique identifier of this bug in its associated bug-tracking system.

`title`  

Optionally, the human-readable title of the bug.

## Return Value

An instance of Bug representing the specified bug.

## Mentioned in 

Associating bugs with tests

Interpreting bug identifiers

Enabling and disabling tests

## See Also

### Annotating tests

Adding tags to tests

Use tags to provide semantic information for organization, filtering, and customizing appearances.

Adding comments to tests

Add comments to provide useful information about tests.

Associating bugs with tests

Associate bugs uncovered or verified by tests.

Interpreting bug identifiers

Examine how the testing library interprets bug identifiers provided by developers.

macro Tag()

Declare a tag that can be applied to a test function or test suite.

static func bug(String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: String, Comment?) -> Self

Construct a bug to track with a test.

