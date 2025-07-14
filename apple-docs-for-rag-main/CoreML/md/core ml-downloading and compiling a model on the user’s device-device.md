

- Core ML
-  Downloading and Compiling a Model on the User’s Device 

Article

# Downloading and Compiling a Model on the User’s Device

Install Core ML models on the user’s device dynamically at runtime.

## Overview

Download and compile models within your app as an alternative to bundling with the app. Scenarios where this is a practical approach include:

- Reducing the app’s download size of your app on the App Store

- Determining the right models for the user after installation based on their location, specific interests, and A/B testing

- Providing model updates over the network

### Download and Compile the Model in the Background

Download the model definition file (ending in `.mlmodel`) onto the user’s device by using URLSession, CloudKit, or another networking toolkit. Then compile the model definition by calling compileModel(at:).

```
```

This creates a new, compiled model file with the same name as the model description but ending in `.mlmodelc`. Create a new MLModel instance by passing the compiled model URL to its initializer.

```
```

Model instances you create from model files you’ve downloaded have the same capabilities as those you create from model files that you bundle with your app.

### Save Reusable Models to a Permanent Location

MLModel saves models it compiles to a temporary location. If your app can reuse the model later, reduce your resource consumption by saving the compiled model to a permanent location.

Build the URL to a permanent location that your app can access in the future, such as Application Support.

```
```

Create the URL for the permanent compiled model file.

```
```

Move or copy the file to its permanent location.

```
```

Important

You should consider the user’s iCloud Backup size when saving large, compiled Core ML models. You can store models in the app’s container using /tmp and /Library/Caches directories, which contain purgeable data that isn’t backed up. When the models aren’t purgeable, you can exclude them from backup by setting the isExcludedFromBackup resource value to `true`. To learn more about excluding files from iCloud Backup, see Optimizing Your App’s Data for iCloud Backup.

## See Also

### Related Documentation

class func compileModel(at: URL) throws -> URL

Compiles a model on the device to update the model in your app.

Deprecated

### App integration

Model Integration Samples

Integrate tabular, image, and text classifcation models into your app.

