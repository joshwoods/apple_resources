

- Swift Testing
- Traits
-  Adding comments to tests 

Article

# Adding comments to tests

Add comments to provide useful information about tests.

## Overview

It’s often useful to add comments to code to:

- Provide context or background information about the code’s purpose

- Explain how complex code implemented

- Include details which may be helpful when diagnosing issues

Test code is no different and can benefit from explanatory code comments, but often test issues are shown in places where the source code of the test is unavailable such as in continuous integration (CI) interfaces or in log files.

Seeing comments related to tests in these contexts can help diagnose issues more quickly. Comments can be added to test declarations and the testing library will automatically capture and show them when issues are recorded.

## Add a code comment to a test

To include a comment on a test or suite, write an ordinary Swift code comment immediately before its `@Test` or `@Suite` attribute:

```
// Assumes the standard lunch menu includes a taco
@Test func lunchMenu() {
  let foodTruck = FoodTruck(
    menu: .lunch,
    ingredients: [.tortillas, .cheese]
  )
  #expect(foodTruck.menu.contains { $0 is Taco })
}
```

The comment, `// Assumes the standard lunch menu includes a taco`, is added to the test.

The following language comment styles are supported:

| Syntax       | Style                       |
|--------------|-----------------------------|
| `// ...`     | Line comment                |
| `/// ...`    | Documentation line comment  |
| `/* ... */`  | Block comment               |
| `/** ... */` | Documentation block comment |

### Comment formatting

Test comments which are automatically added from source code comments preserve their original formatting, including any prefixes like `//` or `/**`. This is because the whitespace and formatting of comments can be meaningful in some circumstances or aid in understanding the comment — for example, when a comment includes an example code snippet or diagram.

## Use test comments effectively

As in normal code, comments on tests are generally most useful when they:

- Add information that isn’t obvious from reading the code

- Provide useful information about the operation or motivation of a test

If a test is related to a bug or issue, consider using the Bug trait instead of comments. For more information, see Associating bugs with tests.

## See Also

### Annotating tests

Adding tags to tests

Use tags to provide semantic information for organization, filtering, and customizing appearances.

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

static func bug(String?, id: some Numeric, Comment?) -> Self

Construct a bug to track with a test.

