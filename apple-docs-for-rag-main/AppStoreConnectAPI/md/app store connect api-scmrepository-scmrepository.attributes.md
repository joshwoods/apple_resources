

- App Store Connect API
- ScmRepository
-  ScmRepository.Attributes 

Object

# ScmRepository.Attributes

The attributes that describe a Repositories resource.

App Store Connect API 1.5+

``` source
object ScmRepository.Attributes
```

## Properties

`httpCloneUrl`

`uri`

The Git repository’s URL for cloning it using HTTP.

`lastAccessedDate`

`date-time`

The date and time when Xcode Cloud last accessed the repository.

`ownerName`

`string`

The name of the Git repository’s owner.

`repositoryName`

`string`

The name of the Git repository.

`sshCloneUrl`

`uri`

The Git repository’s URL for cloning it using SSH.

## See Also

### Objects

object ScmRepository.Relationships

The relationships of the Repositories resource you included in the request and those on which you can operate.

