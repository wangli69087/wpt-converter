# WPT Convert Tool
This tool contains two python scripts to convert webnn-polyfill tests for testing WPT.

* **wpt_converter.py** is used for converting `.js` sample test files of ops to `.html` test files.

* **wpt_model_converter.py** is used for converting `.js` sample test files of models to `.html` test files.

# Run
## Precondition
* python3 is requried
* Prepare sample test file `.js` files: download webnn-polyfill sample test files from github repository (https://github.com/webmachinelearning/webnn-polyfill/tree/master/test), then run wpt_converter.py/wpt_model_converter.py script.

## Commands
$ python3 wpt_converter.py/wpt_model_converter.py <**.js test files parent dir path> <**.html test files parent dir path>, for example:

```sh
$ python3 wpt_converter.py /home/test/ops_js /home/test/ops_html
$ python3 wpt_model_converter.py /home/test/models_js /home/test/models_html
# generated test files are all under "/home/test/ops_html" or "/home/test/models_html".
```
