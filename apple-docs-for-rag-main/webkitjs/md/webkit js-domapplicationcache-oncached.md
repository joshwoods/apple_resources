

- WebKit JS
- DOMApplicationCache
-  oncached 

Instance Property

# oncached

Sent when the update process finishes for the first time—that is, the first time an application cache is saved.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute EventHandler oncached;
```

## See Also

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

