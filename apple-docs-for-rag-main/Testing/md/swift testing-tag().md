

- Swift Testing
-  Tag() 

Macro

# Tag()

Declare a tag that can be applied to a test function or test suite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@attached(accessor) @attached(peer)
macro Tag()
```

## Mentioned in 

Adding tags to tests

## Overview

Use this tag with members of the Tag type declared in an extension to mark them as usable with tests. For more information on declaring tags, see Adding tags to tests.

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

static func bug(String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: some Numeric, Comment?) -> Self

Construct a bug to track with a test.

