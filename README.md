sourcemap-options
=================

The source map options for the `grunt-contrib` suite.

### Options

#### sourceMap 

Type: `boolean`  
Default: `false`  

Set to true to create a source map. The source map will be created alongside the destination file, and share the same file name with the `.map` extension appended to it.

#### sourceMapName  

Type: `string`  `function`  
Default: `undefined`

To customize the name or location of the generated source map, pass a string to indicate where to write the source map to. If a function is provided, the uglify destination is passed as the argument and the return value will be used as the file name.

_Should this be split out into `sourceMapName` and `sourceMapDir` options?_

#### sourceMapStyle

Type: `string`  
Default: `"Embed"`

Determines the type of source map that is generated. The default value, `embed`, places the content of the sources directly into the map. `link` will reference the original sources in the map as links. `inline` will store the entire map as a data URI in the destination file.

### Resources

* [Source Map Revision 3 Proposal](https://docs.google.com/document/d/1U1RGAehQwRypUTovF1KRlpiOFze0b-_2gc6fAH0KY0k/edit)
