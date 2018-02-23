# SystemVerilog-1800-2012 README

This extension incorporates syntax highlighting and snippet support for `IEEE Std 1800-2012 - SystemVerilog` hardware description language and `Universal Verification Methodology` (UVM) version 1.2.

# Features
* Syntax highlighting and basic syntax checking capabilites for SystemVerilog.
* Scope start end checking for *module-endmodule*, *fork-join*, *begin-end*, etc.
* UVM class and type integration ()
* Snippet support for the verification side of SV and UVM

## · SystemVerilog-2012-1800 ·
* checkers
* classes
* comments, attributes, various conventional highlights (accessors, numbers, etc.)
* constraint blocks
* coverage
* interfaces
* modules
* packages
* programs
* tasks and functions
* user-defined primitives

### SV Snippets
SystemVerilog snippets are available with a `sv_` prefix.

* Containers: sv_module, sv_interface, sv_class
* Language constructs: sv_block_parallel, sv_block_sequential, sv_if, sv_if_blocks, sv_if_blocks_labels

As VS Code uses clever search in words and snippets pressing `sq` will most likely result in `sv_block_sequential` so you don't need to type the whole snippet expression. :)

## · UVM ·
UVM classes, macros and functions are partially supported, implementation is work in progress.

### UVM Snippets
The most common UVM boilerplates are available with an `uvm_` prefix.

* UVM containers: uvm_class_object, uvm_class_object_params, uvm_class_component, uvm_class_component_params
* Macros (field macros are purposely omitted): uvm_macro_info, uvm_macro_warning, uvm_macro_error, uvm_macro_object_utils, etc.
* Phases: uvm_phase_build, uvm_phase_connect, etc.

## · Indentation rules ·
* Indentation rules are added for the common constructs of SystemVerilog (eg.: module-endmodule, begin-end, etc.) for VS Code's `reindent` function
* As VS Code uses tmLanguage (TextMate) styled rules for this, there is no multiline support, eg. block comments can break your indentation if a line starts with begin for example.

## · Extra folding rules ·
* Extra folding (but not indentation) rules are set for SystemVerilog compiler directives (eg.: ifndef-endif, pragma protect begin-end, etc.)
* Similarly to indentation rules, line breaked `` `pragma protect begin`` break this feature.

# Release Notes

## 1.0.0

Initial release of SystemVerilog-1800-2012 for the public domain. The addon lacks a lot of features (yet) and will be further developed during the spring. Nevertheless the extension is fully functional and useable.

# License information

This extension is licensed by the MIT License; **Copyright 2018 by Gergo Vekony**

`Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:`

`The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.`

`THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.`

-----------------------------------------------------------------------------------------------------------