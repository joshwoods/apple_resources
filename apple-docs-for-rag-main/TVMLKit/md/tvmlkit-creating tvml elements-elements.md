

- TVMLKit
-  Creating TVML Elements 

Article

# Creating TVML Elements

Avoid rewriting complex and often used elements by creating a simplified custom element.

## Overview

The TVML template elements ensure structure and consistency between documents. However, there are times when applying the same modification to a particular element across a single or multiple documents becomes unwiedly. One such example is when you need to update an element that contains copyright information. By creating a new element that incorporates these changes, you can avoid having to apply the same modifications to each instance of the element.

### Create Your Customization Class

Your element customization class is where you register any new elements and add the customization code. To start, create a new class that conforms to the TVInterfaceCreating protocol and import the UIKit and TVMLKit frameworks:

```
```

### Register Your New Element

Before you can use a new element in your TVML code, register the element using the registerViewElementClass(_:elementName:) function. Call the registerViewElementClass(_:elementName:) in your class’s `init` function and assign a name to the new element. The JavaScript environment can now recognize the registered element. The following code creates the new TVML element, ``:

```
```

Important

You must register all elements before initializing the TVApplicationController object.

### Customize Your New Element

After registering the new element name, you need to customize the element. Implement the makeView(element:existingView:) function in your custom class. The system automatically calls the makeView(element:existingView:) function for every element in your TVML document. Check for the new element’s name and add the customization code. If the current element is not your new element, you must return `nil`.

```
```

### Access the Shared Interface

To enable your class to communicate with your JavaScript code, associate the class with the shared() interface. Before setting the application controller, set the extendedInterfaceCreator property to an instance of the class inside of the application(_:didFinishLaunchingWithOptions:) function:

```
```

When complete, use the new element in your TVML code like any other element; for example, ``.

## See Also

### Custom Elements

class TVElementFactory

An object used to register new elements to extend the Apple TV Markup Language (TVML).

Deprecated

class TVImageElement

A representation of a read-only DOM node containing the attributes that describe an image element.

Deprecated

class TVTextElement

The textual content for the DOM element.

Deprecated

