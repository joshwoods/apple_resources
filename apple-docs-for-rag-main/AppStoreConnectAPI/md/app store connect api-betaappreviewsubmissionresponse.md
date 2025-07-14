

- App Store Connect API
-  BetaAppReviewSubmissionResponse 

Object

# BetaAppReviewSubmissionResponse

A response that contains a single Beta App Review Submissions resource.

App Store Connect API 1.0+

``` source
object BetaAppReviewSubmissionResponse
```

## Properties

`data`

BetaAppReviewSubmission

 (Required) 

The resource data.

`links`

DocumentLinks

 (Required) 

Navigational links that include the self-link.

`included`

`[`Build`]`

## See Also

### Related Documentation

Submit an App for Beta Review

Submit an app for beta app review to allow external testing.

### Objects and Data Types

object BetaAppReviewSubmission

The data structure that represents a Beta App Review Submissions resource.

object BetaAppReviewSubmissionCreateRequest

The request body you use to create a Beta App Review Submission.

object BetaAppReviewSubmissionWithoutIncludesResponse

object BetaAppReviewSubmissionsResponse

A response that contains a list of Beta App Review Submission resources.

type BetaReviewState

String that indicates the review state of a beta app.

