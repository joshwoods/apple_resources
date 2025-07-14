

- App Store Connect API
- CiBuildRun
- CiBuildRun.Attributes
-  CiBuildRun.Attributes.DestinationCommit 

Object

# CiBuildRun.Attributes.DestinationCommit

The latest commit of a pull request’s target branch or the source commit for builds that aren’t pull request builds.

App Store Connect API 1.5+

``` source
object CiBuildRun.Attributes.DestinationCommit
```

## Properties

`author`

CiGitUser

The author of the commit.

`commitSha`

`string`

The commit hash.

`committer`

CiGitUser

The commit’s Git committer.

`message`

`string`

The commit message.

`webUrl`

`uri`

The commit URL.

## See Also

### Objects and Types

object CiBuildRun.Attributes.SourceCommit

The latest commit of a Git branch or tag, or of a pull request’s source branch.

object CiGitUser

The data structure that represents a Git Users resource.

object CiIssueCounts

The data structure that represents an Issue Counts resource.

type CiCompletionStatus

A string that represents the completion status of an Xcode Cloud build.

type CiExecutionProgress

A string that represents the progress of an ongoing Xcode Cloud build.

