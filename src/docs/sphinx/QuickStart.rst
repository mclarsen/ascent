.. ############################################################################
.. # Copyright (c) 2014-2018, Lawrence Livermore National Security, LLC.
.. # 
.. # Produced at the Lawrence Livermore National Laboratory
.. # 
.. # LLNL-CODE-666778
.. # 
.. # All rights reserved.
.. # 
.. # This file is part of Conduit. 
.. # 
.. # For details, see: http://software.llnl.gov/conduit/.
.. # 
.. # Please also read conduit/LICENSE
.. # 
.. # Redistribution and use in source and binary forms, with or without 
.. # modification, are permitted provided that the following conditions are met:
.. # 
.. # * Redistributions of source code must retain the above copyright notice, 
.. #   this list of conditions and the disclaimer below.
.. # 
.. # * Redistributions in binary form must reproduce the above copyright notice,
.. #   this list of conditions and the disclaimer (as noted below) in the
.. #   documentation and/or other materials provided with the distribution.
.. # 
.. # * Neither the name of the LLNS/LLNL nor the names of its contributors may
.. #   be used to endorse or promote products derived from this software without
.. #   specific prior written permission.
.. # 
.. # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
.. # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
.. # IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
.. # ARE DISCLAIMED. IN NO EVENT SHALL LAWRENCE LIVERMORE NATIONAL SECURITY,
.. # LLC, THE U.S. DEPARTMENT OF ENERGY OR CONTRIBUTORS BE LIABLE FOR ANY
.. # DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL 
.. # DAMAGES  (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
.. # OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
.. # HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, 
.. # STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
.. # IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
.. # POSSIBILITY OF SUCH DAMAGE.
.. # 
.. ############################################################################

.. _quick_start:

================================
Quick Start
================================


Installing Ascent and Third Party Dependencies 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The quickest path to install Ascent and its dependencies is via :ref:`uberenv <building_with_uberenv>`:

.. code:: bash
    
    git clone --recursive https://github.com/alpine-dav/ascent.git
    cd ascent
    python scripts/uberenv/uberenv.py --install --prefix="build"


After this completes, ``build/ascent-install`` will contain an Ascent install.

For more details about building and installing Ascent see :ref:`building`. This page provides detailed info about Ascent's CMake options, :ref:`uberenv <building_with_uberenv>` and :ref:`Spack <building_with_spack>` support. We also provide info about :ref:`building for known HPC clusters using uberenv <building_known_hpc>` and a :ref:`Docker example <building_with_docker>` that leverages Spack.


Using Ascent in Your Project
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The install includes examples that demonstrate how to use Ascent in a CMake-based build system  and via a Makefile.

CMake-based build system example (see: ``examples/ascent/using-with-cmake``):

.. literalinclude:: ../../examples/using-with-cmake/CMakeLists.txt 
   :lines: 46-69
   :dedent: 2


Makefile-based build system example (see: ``examples/ascent/using-with-make``):

.. literalinclude:: ../../examples/using-with-make/Makefile
   :lines: 46-61
   :dedent: 2







