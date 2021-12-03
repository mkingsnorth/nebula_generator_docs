#################
Control Panel
#################

.. figure:: ../_static/control_panel_highlight.jpg
    :alt: Nebula Generator
    :width: 100%


The Nebula Generator comes with a control panel that can manage all aspects of the nebula .blend file.

The panel works for both :ref:`Eevee` and :ref:`Cycles` versions.  

It needs to be :ref:`installed<Installing the Panel>` separately.


.. warning:: 

   The control panel can only be seen if one of the Nebula Generator .blend files are open.
   
   

Installing the Panel
**********************************

#. Go to *Edit* -> *Preferences*.
#. Select the *Add-ons* tab on the left if it is not already.
#. Select the *Install...* button along the top.
#. This will open a file dialog where you should navigate to where you have downloaded the **nebula_generator.x.x.x.zip** file (where x.x.x is the version number).  This file should not be unzipped.
#. Then, click the *Install add-on from file* button.
#. Search for the add-on by typing *Nebula Generator* in the search box if it does not already appear.
#. Make sure the checkbox next to the Add-on (*Add Mesh: Nebula Generator*) is ticked:

.. figure:: ../_static/install_window.jpg
  :alt: Nebula Generator Installed

  Nebula Generator Panel Installed

If you have any issues do not hesitate to get in touch via `info@configurate.net <mailto:info@configurate.net>`_.


Usage
**********************************

.. figure:: ../_static/side_panel_anim.gif
  :alt: Nebula Generator Installed

  Accessing the control panel.



#. Open one of the Nebula Generator's .blend files.  You will not be able to see or use the panel otherwise.
#. If you cannot see any tabs on the left hand side of the viewport, press the 'N' key.
#. Navigate to the tab named "Nebula Generator".  

.. warning:: 

   The control panel works on the nodes and particle systems of the .blend file.  Adding or Deleting the nodes or particles will stop the panel from working.

See the :ref:`troubleshooting` section if you are having issues and don't hesitate to :ref:`get in touch<contact>`

Panel Controls
**********************************

Each section controls a different aspect of the nebula:

Stars
=============================

.. figure:: ../_static/controls_stars.jpg
  :alt: Nebula Generator Controls

This controls the number and random placement of the stars.

Large stars
------------------

.. figure:: ../_static/large_stars.jpg
  :alt: Large Stars

The Large Stars are actually point like sources that light the nebula.

* **Number**:  The number of large stars in the nebula.  Their number is set relatively low as too many and the lights will become overwhelming.
* **Seed**: This is a seed value to control the random placement of the stars.  Changing this number will randomly place the stars in different positions.

Small stars
------------------

.. figure:: ../_static/small_stars.jpg
  :alt: Small Stars

The smaller stars do not actually emit light and are exist to proved background and depth.

* **Number**:  The number of small stars in the nebula.
* **Seed**: This is a seed value to control the random placement of the stars.  Changing this number will randomly place the stars in different positions.
* **Size**: The size of the small stars.


Colors
=============================

.. figure:: ../_static/colors_anim.gif
  :alt: Changing Colors

Change the colors of the lighting, clouds and small stars separately:

Lighting
------------------

.. figure:: ../_static/lighting_panel.jpg
  :alt: Lighting Panel

This controls the light emitted from the :ref:`Large Stars`.

* **Color**: The color of the lights.
* **Power**: How powerful these lights/stars are.

Clouds and Small Stars
-------------------------

Main Cloud
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


.. figure:: ../_static/main_cloud_colors.gif
  :alt: Main Cloud Colors
  :width: 100%

.. figure:: ../_static/main_cloud_colors.jpg
  :alt: Main Cloud Colors

* **Color Ramp**: This is a |color ramp| control to change the color of the thickest clouds.  Values on the left hand side of the ramp controls the colors of the least dense part of those clouds, where values on the right control the most dense parts.
* **Hue/Sat/Val**: This alters the hue, saturation and value of the ramp color.  Colors changes will be shown in the viewport, but not on the ramp controls.

.. |color ramp| raw:: html

   <a href="https://docs.blender.org/manual/en/latest/modeling/geometry_nodes/color/color_ramp.html" target="_blank"><b>color ramp</b></a>




Cloud Gas
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. figure:: ../_static/gas_cloud_colors.gif
  :alt: Gas Cloud Colors
  :width: 100%

.. figure:: ../_static/gas_cloud_colors.jpg
  :alt: Gas Cloud Colors

* **Color Ramp**: This is a |color ramp| control to change the color of the lighter clouds that surround the denser clouds.  Values on the left hand side of the ramp controls the colors of the least dense part of those clouds, where values on the right control the most dense parts.
* **Hue/Sat/Val**: This alters the hue, saturation and value of the ramp color.  Colors changes will be shown in the viewport, but not on the ramp controls.


Small Stars Colors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



.. figure:: ../_static/small_stars_colors.gif
  :alt: Small Stars Colors
  :width: 100%

.. figure:: ../_static/small_stars_colors.jpg
  :alt: Small Stars Colors

* **Color Ramp**: This is a |color ramp| control to change the different colors of the small background stars.  The range of colors along the ramp are randomly assigned to each star.
* **Hue/Sat/Val**: This alters the hue, saturation and value of the colors.  Colors changes will be shown in the viewport, but not on the ramp controls.

Overall Hue/Saturation/Value
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. figure:: ../_static/overall_hsv.gif
  :alt: Small Stars Colors
  :width: 100%

.. figure:: ../_static/overall_hsv.jpg
  :alt: Overall Hue/Saturation/Value

This controls the overall Hue, Saturation and Value of the clouds and small stars. This is useful if you are happy with the overall values that are set.  Note the lighting is altered separately.

.. tip:: 

    .. figure:: ../_static/expand_panel.gif
        :alt: Main Cloud Colors

   You can expand the width of the panel so you have more room to control the color ramps.


Density
=============================

Noise
=============================

Transform
=============================

Quality
=============================
