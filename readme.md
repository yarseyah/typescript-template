<h1>Typescript template for VS Code</h1>

<h2>Layout</h2>
The following structure is used for the template

```
<root>
	<.settings> - VS Code tasks are defined here
	<src>
		<js> - files are automatically generated in here
		<ts> - this is where the source typescript files are created
	<typings>
		(stuff here is to support the .d.ts creation)
	(files here are for the management of node, gulp, tsd, tslint, etc.)
```

<h2>References</h2>
Quite a lot of the approach to this came from my following this guide: http://weblogs.asp.net/dwahlin/creating-a-typescript-workflow-with-gulp
In the end, it did more than I wanted to do which was to just have an environment with the basic tooling set up (e.g. didn't want bower, etc).
