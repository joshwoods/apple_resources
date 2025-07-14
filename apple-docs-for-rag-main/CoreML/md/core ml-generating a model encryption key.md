

- Core ML
-  Generating a Model Encryption Key 

Article

# Generating a Model Encryption Key

Create a model encryption key to encrypt a compiled model or model archive.

## Overview

Use a model’s encryption key to encrypt a model archive for deployment or to encrypt a model compiled and bundled into your app.

Important

You must have signed in with your Apple ID in the Apple ID pane in System Preferences to generate a model encryption key in Xcode.

### Create the Model Encryption Key

Open a model in Xcode, click the Utilities tab, and click Create Encryption Key.

Select the development team that your app’s target uses from the menu, and click Continue.

Xcode’s confirmation dialog provides an arrow button that takes you to the encryption key in Finder.

### Locate the Model Encryption Key

Use the first button in the confirmation dialog to show the model encryption key in Finder, or navigate to the model’s enclosing folder.

Xcode saves the model encryption key file in the same folder as the original model file, and uses its base name with the `.mlmodelkey` extension. For example, the encryption key for a model named `Classifier.mlmodel` has the name `Classifier.mlmodelkey` in the same directory.

Use this model encryption file to:

- Encrypt a model archive as you generate it using Xcode (see `Generating a Model Archive`).

- Encrypt a model that Xcode includes in your app’s bundle as it compiles the model (see Encrypting a Model in Your App).

## See Also

### Model encryption

Encrypting a Model in Your App

Encrypt your app’s built-in model at compile time by adding a compiler flag.

