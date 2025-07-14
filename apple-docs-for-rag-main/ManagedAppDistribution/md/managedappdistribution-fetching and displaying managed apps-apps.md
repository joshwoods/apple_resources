

- ManagedAppDistribution
-  Fetching and displaying managed apps 

Article

# Fetching and displaying managed apps

Provide a consistent app presentation when displaying managed apps.

## Overview

Your app can take advantage of Managed App Distribution features to display download status and launch apps. Obtain a list of ManagedApp objects, then display that list of apps in a custom view.

### Fetching

This code snippet defines a model that obtains a list of apps from a ManagedAppLibrary.

```
```

### Displaying

After you fetch the list of apps from the model, display them in a compact content style within your custom view.

This code snippet demonstrates how to display the list of apps.

```
```

## See Also

### Essentials

struct ManagedApp

A representation of a managed app.

class ManagedAppLibrary

A representation of a library of managed apps.

