

- App Store Connect API
- ScmRepository
-  ScmRepository.Relationships 

Object

# ScmRepository.Relationships

The relationships of the Repositories resource you included in the request and those on which you can operate.

App Store Connect API 1.5+

``` source
object ScmRepository.Relationships
```

## Properties

`defaultBranch`

ScmRepository.Relationships.DefaultBranch

The Git repository’s default branch.

`gitReferences`

ScmRepository.Relationships.GitReferences

`pullRequests`

ScmRepository.Relationships.PullRequests

`scmProvider`

ScmRepository.Relationships.ScmProvider

The related Providers resource.

## Topics

### Objects

object ScmRepository.Relationships.DefaultBranch

The data and links that describe the relationship between the Repositories resource and the Git References resource that represents the default branch.

object ScmRepository.Relationships.ScmProvider

The data and links that describe the relationship between the Repositories and the Source Code Management Provider resources.

### Dictionaries

object ScmRepository.Relationships.GitReferences

object ScmRepository.Relationships.PullRequests

## See Also

### Objects

object ScmRepository.Attributes

The attributes that describe a Repositories resource.

