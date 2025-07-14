

- App Store Connect API
-  BetaAppReviewSubmissionsResponse 

Object

# BetaAppReviewSubmissionsResponse

A response that contains a list of Beta App Review Submission resources.

App Store Connect API 1.0+

``` source
object BetaAppReviewSubmissionsResponse
```

## Properties

`data`

`[`BetaAppReviewSubmission`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

`included`

`[`Build`]`

## See Also

### Related Documentation

List Beta App Review Submissions

Find and list beta app review submissions for all builds.

### Objects and Data Types

object BetaAppReviewSubmission

The data structure that represents a Beta App Review Submissions resource.

object BetaAppReviewSubmissionCreateRequest

The request body you use to create a Beta App Review Submission.

object BetaAppReviewSubmissionResponse

A response that contains a single Beta App Review Submissions resource.

object BetaAppReviewSubmissionWithoutIncludesResponse

type BetaReviewState

String that indicates the review state of a beta app.

