

- Core ML
-  Encrypting a Model in Your App 

Article

# Encrypting a Model in Your App

Encrypt your app’s built-in model at compile time by adding a compiler flag.

## Overview

Tell Xcode to encrypt your model as it compiles your app by adding a compiler flag to your build target.

### Add a Compiler Flag

In Xcode, navigate to your project’s target and open its Build Phases tab. Expand the Compile Sources section and select the model you want Xcode to encrypt at compile time. Open the model’s compiler flags editor by double-clicking the model’s entry.

In the editor, add:

1.  The encryption flag “`--encrypt`”

2.  A space character

3.  The absolute path to the model’s encryption key file you created (see Generating a Model Encryption Key), between quotation marks

Press the Return key or click outside the editor to close it.

### Load the Model

At runtime, you load the encrypted model the same way you load any other built-in model by using its `load(completionHandler:completionHandler:)` type method. This method behaves similarly to the MLModel type method loadContentsOfURL:configuration:completionHandler: and creates an instance of the model using the convenience class that Xcode generates.

## See Also

### Model encryption

Generating a Model Encryption Key

Create a model encryption key to encrypt a compiled model or model archive.

