d3-externs
==========

Full ClojureScript extern file for the [D3][1] (version 3.0.6)
library. It allows to use D3 library under the Google Closure's
advanced optimization.


## Usage

Download `d3_externs.js` and place it in your leiningen project
folder, say `./externs/d3_externs.js`. Set the externs in the compiler
options of the project as shown below

```clj
	:your-build-name {:source-paths ["src/cljs"]
		              :compiler {:output-to "resources/public/js/modern.js"
                                 :optimizations :advanced
								 :externs ["externs/d3_externs.js"]}}
```

### Compatibility

All `lein-cljsbuild` versions supporting `:externs` options. 

[1]: http://www.d3js.org
