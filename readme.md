<h1>Typescript template for VS Code</h1>

<h2>Overview</h2>
The template has been set up to include:
* Typescript
* Typescript-definitions ( *.d.ts )
* Typescript Linting (tslint)
* Create source-maps from the JS back to the original TS

It uses nodejs and gulp to automatically process any typescript files (Created in the `src\ts\` folder) and convert them to JavaScript (in the `src\js\` folder).

The Visual Studio Code task has been wired up to perform the default Gulp task, which does the following (just press <kbd>Control</kbd>-<kbd>Shift</kbd>+<kbd>B</kbd>):
* Lint (check the basic coding style)
* Compile
* Update the definition references
* Watch for future TS changes.

<h2>Getting started</h2>
Download the ZIP of the template to the directory you which to develop in:
* Ensure you have nodejs/npm on your search-path 
* Type `npm install` to restore runtime and development dependencies

<h2>Layout</h2>
The following structure is used for the template

```
<root>
│─── .settings         VS Code tasks are defined here
│─── src
│  │─── js             files are automatically generated in here
│  └─── ts             this is where the source typescript files are created
└─── typings	       stuff below here is to support the .d.ts creation
(files here are for the management of node, gulp, tsd, tslint, etc.)
```

<h2>References</h2>
Quite a lot of the approach to this came from my following this guide: http://weblogs.asp.net/dwahlin/creating-a-typescript-workflow-with-gulp
In the end, it did more than I wanted to do which was to just have an environment with the basic tooling set up (e.g. didn't want bower, etc).
