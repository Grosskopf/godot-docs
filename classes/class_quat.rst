.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Quat.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Quat:

Quat
====

**Category:** Built-In Types

Brief Description
-----------------

Quaternion.

Member Functions
----------------

+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`Quat<class_Quat_Quat>` **(** :ref:`float<class_float>` x, :ref:`float<class_float>` y, :ref:`float<class_float>` z, :ref:`float<class_float>` w **)**                  |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`Quat<class_Quat_Quat>` **(** :ref:`Vector3<class_vector3>` axis, :ref:`float<class_float>` angle **)**                                                                 |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`Quat<class_Quat_Quat>` **(** :ref:`Basis<class_basis>` from **)**                                                                                                      |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`cubic_slerp<class_Quat_cubic_slerp>` **(** :ref:`Quat<class_quat>` b, :ref:`Quat<class_quat>` pre_a, :ref:`Quat<class_quat>` post_b, :ref:`float<class_float>` t **)** |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`      | :ref:`dot<class_Quat_dot>` **(** :ref:`Quat<class_quat>` b **)**                                                                                                             |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`inverse<class_Quat_inverse>` **(** **)**                                                                                                                               |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`        | :ref:`is_normalized<class_Quat_is_normalized>` **(** **)**                                                                                                                   |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`      | :ref:`length<class_Quat_length>` **(** **)**                                                                                                                                 |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`      | :ref:`length_squared<class_Quat_length_squared>` **(** **)**                                                                                                                 |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`normalized<class_Quat_normalized>` **(** **)**                                                                                                                         |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`slerp<class_Quat_slerp>` **(** :ref:`Quat<class_quat>` b, :ref:`float<class_float>` t **)**                                                                            |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Quat<class_quat>`        | :ref:`slerpni<class_Quat_slerpni>` **(** :ref:`Quat<class_quat>` b, :ref:`float<class_float>` t **)**                                                                        |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_vector3>`  | :ref:`xform<class_Quat_xform>` **(** :ref:`Vector3<class_vector3>` v **)**                                                                                                   |
+--------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_Quat_w:

- :ref:`float<class_float>` **w**

  .. _class_Quat_x:

- :ref:`float<class_float>` **x**

  .. _class_Quat_y:

- :ref:`float<class_float>` **y**

  .. _class_Quat_z:

- :ref:`float<class_float>` **z**


Description
-----------

Quaternion is a 4 dimensional vector that is used to represent a rotation. It mainly exists to perform SLERP (spherical-linear interpolation) between two rotations. Multiplying quaternions also cheaply reproduces rotation sequences. However quaternions need to be often renormalized, or else they suffer from precision issues.

Member Function Description
---------------------------

.. _class_Quat_Quat:

- :ref:`Quat<class_quat>` **Quat** **(** :ref:`float<class_float>` x, :ref:`float<class_float>` y, :ref:`float<class_float>` z, :ref:`float<class_float>` w **)**

.. _class_Quat_Quat:

- :ref:`Quat<class_quat>` **Quat** **(** :ref:`Vector3<class_vector3>` axis, :ref:`float<class_float>` angle **)**

Returns a quaternion that will rotate around the given axis by the specified angle. The axis must be a normalized vector.

.. _class_Quat_Quat:

- :ref:`Quat<class_quat>` **Quat** **(** :ref:`Basis<class_basis>` from **)**

Returns the rotation matrix corresponding to the given quaternion.

.. _class_Quat_cubic_slerp:

- :ref:`Quat<class_quat>` **cubic_slerp** **(** :ref:`Quat<class_quat>` b, :ref:`Quat<class_quat>` pre_a, :ref:`Quat<class_quat>` post_b, :ref:`float<class_float>` t **)**

.. _class_Quat_dot:

- :ref:`float<class_float>` **dot** **(** :ref:`Quat<class_quat>` b **)**

Returns the dot product of two quaternions.

.. _class_Quat_inverse:

- :ref:`Quat<class_quat>` **inverse** **(** **)**

Returns the inverse of the quaternion.

.. _class_Quat_is_normalized:

- :ref:`bool<class_bool>` **is_normalized** **(** **)**

Returns whether the quaternion is normalized or not.

.. _class_Quat_length:

- :ref:`float<class_float>` **length** **(** **)**

Returns the length of the quaternion.

.. _class_Quat_length_squared:

- :ref:`float<class_float>` **length_squared** **(** **)**

Returns the length of the quaternion, squared.

.. _class_Quat_normalized:

- :ref:`Quat<class_quat>` **normalized** **(** **)**

Returns a copy of the quaternion, normalized to unit length.

.. _class_Quat_slerp:

- :ref:`Quat<class_quat>` **slerp** **(** :ref:`Quat<class_quat>` b, :ref:`float<class_float>` t **)**

Perform a spherical-linear interpolation with another quaternion.

.. _class_Quat_slerpni:

- :ref:`Quat<class_quat>` **slerpni** **(** :ref:`Quat<class_quat>` b, :ref:`float<class_float>` t **)**

.. _class_Quat_xform:

- :ref:`Vector3<class_vector3>` **xform** **(** :ref:`Vector3<class_vector3>` v **)**


