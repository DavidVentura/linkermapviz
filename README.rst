linkermapviz
============

Interactive visualization of GNU ld’s linker map with a tree map. Usage:

.. code:: bash

   # install
   pip install .
   # example compilation
   gcc -Wl,-Map,output.map -o output input.c
   # example usage
   linkermapviz output.map
   # example usage
   linkermapviz output.map --ignore-files blabla.a

Works best with ``-ffunction-sections -fdata-sections`` and statically linked
code (e.g. for bare-metal embedded systems).

