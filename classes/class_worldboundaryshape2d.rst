:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the WorldBoundaryShape2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_WorldBoundaryShape2D:

WorldBoundaryShape2D
====================

**Inherits:** :ref:`Shape2D<class_Shape2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

World boundary (infinite plane) shape resource for 2D physics.

Description
-----------

2D world boundary shape to be added as a *direct* child of a :ref:`PhysicsBody2D<class_PhysicsBody2D>` or :ref:`Area2D<class_Area2D>` using a :ref:`CollisionShape2D<class_CollisionShape2D>` node. ``WorldBoundaryShape2D`` works like an infinite plane and will not allow any physics body to go to the negative side. Note that the :ref:`normal<class_WorldBoundaryShape2D_property_normal>` matters; anything "below" the plane will collide with it. If the ``WorldBoundaryShape2D`` is used in a :ref:`PhysicsBody2D<class_PhysicsBody2D>`, it will cause colliding objects placed "below" it to teleport "above" the plane.

\ **Performance:** Being a primitive collision shape, ``WorldBoundaryShape2D`` is fast to check collisions against.

Properties
----------

+-------------------------------+---------------------------------------------------------------+--------------------+
| :ref:`float<class_float>`     | :ref:`distance<class_WorldBoundaryShape2D_property_distance>` | ``0.0``            |
+-------------------------------+---------------------------------------------------------------+--------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`normal<class_WorldBoundaryShape2D_property_normal>`     | ``Vector2(0, -1)`` |
+-------------------------------+---------------------------------------------------------------+--------------------+

Property Descriptions
---------------------

.. _class_WorldBoundaryShape2D_property_distance:

- :ref:`float<class_float>` **distance**

+-----------+---------------------+
| *Default* | ``0.0``             |
+-----------+---------------------+
| *Setter*  | set_distance(value) |
+-----------+---------------------+
| *Getter*  | get_distance()      |
+-----------+---------------------+

The line's distance from the origin.

----

.. _class_WorldBoundaryShape2D_property_normal:

- :ref:`Vector2<class_Vector2>` **normal**

+-----------+--------------------+
| *Default* | ``Vector2(0, -1)`` |
+-----------+--------------------+
| *Setter*  | set_normal(value)  |
+-----------+--------------------+
| *Getter*  | get_normal()       |
+-----------+--------------------+

The line's normal. Defaults to ``Vector2.UP``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
