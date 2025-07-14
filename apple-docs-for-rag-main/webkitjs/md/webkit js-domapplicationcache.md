

- WebKit JS
-  DOMApplicationCache 

Class

# DOMApplicationCache

A `DOMApplicationCache` object is used to store resources—such as, HTML, JavaScript, CSS, and images—locally. This allows your web application to continue running offline when there is no network connection. The cache persists after Safari exits, so it can be used by multiple browser sessions. There is one application cache per browsing context.

Safari Desktop 10.0+Safari Mobile 2.1+

``` source
interface DOMApplicationCache
```

## Topics

### Accessing Properties

status

The current status of the application cache. One of the values described in "Constants.”

### Handling Events

onchecking

Sent when the cache update process begins.

onerror

Sent when an error occurs.

onnoupdate

Sent when the update process finishes but the manifest file does not change.

ondownloading

Sent when the update process begins downloading resources in the manifest file.

onprogress

Sent when each resource in the manifest file begins to download.

onupdateready

Sent when there is an existing application cache, the update process finishes, and there is a new application cache ready for use.

oncached

Sent when the update process finishes for the first time—that is, the first time an application cache is saved.

### Updating the Cache

add

Forthcoming

update

Manually triggers the update process.

swapCache

Replaces the active cache with the latest version.

### Constants

Constants that indicate the status of the application cache.

UNCACHED

The object isn’t associated with an application cache. This can occur if the update process fails and there is no previous cache to revert to, or if there is no manifest file.

IDLE

The cache is idle.

CHECKING

The update has started but the resources are not downloaded yet—for example, this can happen when the manifest file is fetched.

DOWNLOADING

The resources are being downloaded into the cache.

UPDATEREADY

Resources have finished downloading and the new cache is ready to be used.

### Instance Properties

onobsolete

### Instance Methods

abort

### Miscellaneous

OBSOLETE

## Relationships

### Inherits From

- EventTarget

