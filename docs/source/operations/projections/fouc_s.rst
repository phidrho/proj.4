.. _fouc_s:

********************************************************************************
Foucaut Sinusoidal
********************************************************************************

.. image:: ./images/fouc_s.png
   :scale: 50%
   :alt:   Foucaut Sinusoidal


The `y`-axis is based upon a weighted mean of the cylindrical equal-area and
the sinusoidal projections. Parameter :math:`n=n` is the weighting factor where
:math:`0 <= n <= 1`.

.. math::

    x &= \lambda \cos \phi / (n + (1 - n) \ cos \phi)

    y &= n \phi + (1 - n) \sin \phi

For the inverse, the Newton-Raphson method can be used to determine
:math:`\phi` from the equation for :math:`y` above. As :math:`n \rightarrow 0` and
:math:`\phi \rightarrow \pi/2`, convergence is slow but for :math:`n = 0`, :math:`\phi =
\sin^1y`


Parameters
################################################################################

.. note:: All parameters are optional for the Foucaut Sinusoidal projection.

.. option:: +n=<value>

    Weighting factor. Value should be in the interval 0-1.

.. include:: ../options/lon_0.rst

.. include:: ../options/R.rst

.. include:: ../options/x_0.rst

.. include:: ../options/y_0.rst
