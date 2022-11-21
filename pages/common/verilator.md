# verilator

> Converts Verilog and SystemVerilog hardware description language (HDL) designs into a C++ or SystemC model that after compiling can be executed.
> More information: <https://veripool.org/guide/latest/>.

- Build the C project in the current directory:

`verilator --binary -j 0 -Wall {{path/to/source.v}}`

- Create C++ executable:

`verilator --cc --exe --build -j 0 -Wall {{path/to/source.cpp}} {{path/to/output.v}}`

- Perform linting over the code in the current directory:

`verilator --lint-only -Wall`

- Create XML output about the design (files, modules, instance hierarchy, logic and data types) to feed into other tools:

`verilator --xml-output {{path/to/output.xml}} -Wall`
