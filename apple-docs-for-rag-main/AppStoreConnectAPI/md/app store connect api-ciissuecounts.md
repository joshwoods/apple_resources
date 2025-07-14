

- App Store Connect API
-  CiIssueCounts 

Object

# CiIssueCounts

The data structure that represents an Issue Counts resource.

App Store Connect API 1.5+

``` source
object CiIssueCounts
```

## Properties

`analyzerWarnings`

`integer`

The number of analyzer warnings.

`errors`

`integer`

The number of errors.

`testFailures`

`integer`

The number of failing tests.

`warnings`

`integer`

The number of warnings.

## See Also

### Objects and Types

object CiBuildRun.Attributes.DestinationCommit

The latest commit of a pull request’s target branch or the source commit for builds that aren’t pull request builds.

object CiBuildRun.Attributes.SourceCommit

The latest commit of a Git branch or tag, or of a pull request’s source branch.

object CiGitUser

The data structure that represents a Git Users resource.

type CiCompletionStatus

A string that represents the completion status of an Xcode Cloud build.

type CiExecutionProgress

A string that represents the progress of an ongoing Xcode Cloud build.

