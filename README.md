# Anchor SPA

Creates a single-page application using the CSS `:target` selector to hide and show pages.

## Installation

- Requires Python 3.6

Clone or download this project to wherever you like. 

## Use

You can create .template files in the /templates directory. These template files can be referenced in other templates to link between "pages" of your SPA by using anchors with the ID being the filename of the template. For instance, 

```html
<a href="#second">Go to a second page</a>
```
will link to the second.template file. 

There are a number of default assets included which are used for demonstration. You can delete these if you feel like it and replace them with your own files.

When you're done, run `./anchor-build`. This will create an index.html file in the /build directory, and also copy over the assets, scripts and styles folders to it.

## Configuration

The config.json file contains certain configuration values that used to build the project.

-  `head`: contains the `<head>` that will be used on your SPA. By default this is head.template. 

-  `lang`: sets the HTML lang in the index.html output. By default this is 'en'. 

-  `main`: contains the template that will be shown when the user opens the site without navigating to any links. By default this is index.template. 
