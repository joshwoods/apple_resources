

- CloudKit JS
- CloudKit
-  configure 

Instance Method

# configure

Configures CloudKit JS.

CloudKit JS 1.0+

``` source
CloudKit configure(
 CloudKit.CloudKitConfig config
);
```

## Parameters 

`config`  

The properties to use to initialize CloudKit JS.

## Return Value

The configured CloudKit object.

## Discussion

For each container that you access, specify the container ID, API token, and environment.

```
CloudKit.configure({
    containers: [{
        containerIdentifier: '[insert your container ID here]',
        apiTokenAuth: {
            apiToken: '[insert your API token and other authentication properties here]'
        },
        environment: 'development'
    }]
});
```

Other CloudKit.ContainerConfig.`apiTokenAuth` keys, such as the `persist` key, are optional. To keep the user signed in after closing and reopening the browser, set `persist` to `true`.

```
CloudKit.configure({
    containers: [{
        // ...
        apiTokenAuth: {
            apiToken: '[insert your API token and other authentication properties here]',
            persist: true
        }
    }]
});
```

To customize the sign in and sign out buttons, add `signInButton` and `signOutButton` keys to the `auth` dictionary.

For more container and service configuration options, see CloudKit.CloudKitConfig in CloudKit JS Data Types.

