Clj3D - Visual prototyping for the masses
=========================================

This is a fork from the original [https://github.com/adinapoli/clj3D](https://github.com/adinapoli/clj3D).

Currently mostly planning to bring it to speed with Leiningen 2 and Clojure 1.5

Clj3D is a Clojure graphic library for manipulating 3D and 2D objects. It
aims to be the Clojure standard in 3D and 2D rendering. 


..Clj3D is jMonkeyEngine and Plasm reloaded
-------------------------------------------
Clj3D is massively based on the excellent `jMonkeyEngine <http://jmonkeyengine.org/>`_ 
and it tooks the best of it. `PLaSM <http://www.dia.uniroma3.it/~paoluzzi/plasm502/>`_
is a "design language" for geometric and solid parametric design, developed by the 
CAD Group at the Universities "La Sapienza" and "Roma Tre".\

..Clj3D is easy to start with
-----------------------------
No external dependencies, no modules to install. Just a single jar:
::

[hellonico/clj3d "0.0.5"]

Import it into a Leiningen project and you are ready to go. Displaying something is dead-easy:
::

    (use '(clj3D math fl fenvs viewer) :reload)
    (view (cube 1))

..Clj3D is batteries included
-----------------------------
Clj3D is shipped with some interesting library and features, like the powerful
`Incanter <http://incanter.org/>`_ library. Clj3D offers to you the best features
of this library directly injected into the namespace. Forget external ":use" or
":require". You can even use some Incanter methods:
::

  (view (matrix [[0 1 2] 
                 [3 4 5]]))

..Clj3D is fast (as it can)
---------------------------
Clojure is not (unfortunately) written in C, but Java can be relatively fast. Clj3D
tries to be as fast as Java native code, using vectors as primary data structures and
Incanter's matrix when they needs.

..Clj3D is free
---------------
Clj3D is free and it's hosted on `Github <https://github.com/CharlesStain/clj3D>`_

Distributed under the MIT License. JMonkey3 is released under the BSD License. See Wiki.
