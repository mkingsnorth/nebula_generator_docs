##############
Eevee
##############

.. figure:: ../_static/eevee_version.gif
  :alt: Nebula Generator
  :width: 100%


The EEVEE version allows you to quickly generate and position the nebula.  

*****************
Advantages
*****************
* Faster than Cycles.
* Quickly visualise the effect in the viewport.
* Best at still shots and backgrounds

*****************
Disadvantages
*****************
* When animating, a strobing effect can occur.  This is because EEVEE converts the nebula to flat 2D cards when rendering.  The :ref:`Cycles<Cycles>` version does not have this issue.
* Edges of the clouds can appear slightly blurred, which can be sharpened if you can :ref:`change Blender's code slightly<Decreasing Time Size>`.