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


Using the Control Panel
**********************************

.. figure:: ../_static/side_panel_anim.gif
  :alt: Nebula Generator Installed

  Accessing the control panel.



#. Open one of the Nebula Generator's .blend files.  You will not be able to see or use the panel otherwise.
#. If you cannot see any tabs on the left hand side of the viewport, press the 'N' key.
#. Navigate to the tab named "Nebula Generator".  

.. tip::
    Using the shift key whilst dragging the mouse over the parameters will provide a higher degree of control.

.. warning:: 

   The control panel works on the nodes and particle systems of the .blend file.  Adding or Deleting the nodes or particles will stop the panel from working.

See the :ref:`faq` section if you are having issues and don't hesitate to :ref:`get in touch<contact>`

Control Panel Parameters
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

.. image:: ../_static/main_cloud_density.gif
  :alt: Cloud Density

Control the different densities and sizes of the nebula's cloud and gas.

Main Cloud Density
------------------------------------

.. image:: ../_static/main_cloud_density.jpg
  :alt: Cloud Density


This controls the density of the main clouds. 

The |color ramp| controls where the cloud starts and ends.  The white part of the gradient ramp will be the thickest part of the cloud and the black parts will have no cloud at all.  Try dragging different parts of the gradient to get different effects, or by adding or removing different control points on the gradient.

The **Density Multiplier** increases the thickness of the clouds even further.


Cloud Gas Density
------------------------------------

.. image:: ../_static/gas_cloud_density.jpg
  :alt: Cloud Density


This controls the density of the gas surrounding the clouds.  The |color ramp| controls where the cloud starts and ends.  The white parts of the gradient ramp will be the thickest part of the gas and the black parts will have no clouds at all.

The **Density Multiplier** increases the thickness of the clouds even further.

Noise
=============================

.. image:: ../_static/noise_changing.gif
  :alt: Changing the Noise


The cloud shapes are generated using a set of |noise nodes| overlayed on top of each other.  See |this article| for how noise functions are used in computer graphics.

To get a variety of effects, changing the parameters here will change the different inputs to those |noise nodes|.  

.. tip:: 

    If you wish to have even greater control, try changing the noise node set-up in the "Shape" section of the shader tab.  However, this section of the control panel will no longer work properly as it is tied to the existing node setup.

.. |this article| raw:: html

   <a href="https://en.wikipedia.org/wiki/Perlin_noise" target="_blank"><b>this article</b></a>

.. |noise nodes| raw:: html

   <a href="https://docs.blender.org/manual/en/latest/render/shader_nodes/textures/noise.html" target="_blank"><b>noise functions</b></a>


Overall Noise
------------------------------------

This controls the overall noise being applied.

* **Detail**: Number of noise octaves or waves, creating more variation in the clouds. Higher number of octaves corresponds to a higher render time.

    .. image:: ../_static/overall_detail_control.gif
        :alt: Changing the Noise

* **Roughness**: Number of 'peaks' in the noise, where higher values will provide rougher surface effects.

    .. image:: ../_static/overall_roughness_control.gif
        :alt: Changing the Noise

Noise Scale Variation
------------------------------------

The 'Size', or 'Scale', of the overall noise effect is manipulated even further by another noise function to give a more dynamic effect.

.. image:: ../_static/noise_scale_var_control.gif
    :alt: Changing the Noise

* **Scale**:  The size of the noise effect that is used to manipulate the overall scale.
* **Detail**: Number of noise octaves or waves, creating more variation in the scale of the clouds.
* **Roughness**: Number of 'peaks' in the noise used to affect the overall scale of the clouds.
* **Distortion**: The amount of bending or distortion being applied to the overall noise scale.

Noise Distortion Variation
------------------------------------

The 'distortion' of the overall noise is also manipulated by another noise function.  

Although not always apparent in preview mode, this adds a greater level of smaller surface detail to the clouds.  Be careful increasing the parameters such as 'scale' too high or the clouds may appear too noisey at render time:

.. image:: ../_static/noise_distortion_scale_gotcha.jpg
    :alt: Noise distortion gotcha

* **Scale**:  The size of the noise effect that is used to manipulate the overall distortion.
* **Detail**: Number of noise octaves or waves, creating more variation in the distortion of the clouds.
* **Roughness**: Number of 'peaks' in the noise used to affect the overall distortion of the clouds.
* **Distortion**: The amount of bending or distortion being applied to the overall noise distortion.


Transform
=============================

Control the postion of the nebula's location, rotation and scale inside the object:

.. image:: ../_static/noise_transform_control.gif
    :alt: Noise transform control in action

* **Location**: Location of the nebula.
* **Rotation**: Rotation of the nebula's clouds.
* **Scale**: Overall size of the nebula..

Quality
=============================

.. image:: ../_static/quality_control.gif
    :alt: Quality control

Depending on whether you are rendering in Eevee or Cycles, the following parameters expose the most frequently used settings when controlling the quality of the nebula image.  

.. tip::
    These settings and more can be found on the standard Render Properties tab as well, and are provided here for convenience.


* **Render Engine**: Choose between Eevee and Cycles modes.  Not sure which?  See the :ref:`FAQ` section.

    .. image:: ../_static/render_engine_setting.jpg
        :alt: Render Engine Setting

Eevee Quality Settings
------------------------------------

.. image:: ../_static/eevee_quality_settings.jpg
    :alt: Eevee Quality Settings

* **Tile Size**: Arguably one of the most important settings in Eevee volumetric rendering, this controls the level of detail for the render.  The smaller the tile size, the greater level of detail at the expense of memory usage and render times which will also slow down your GPU in Eevee.  Whilst altering the nebula parameters, it is best to keep the setting at either 4px or 8px and then change to 2px for the final render.

    .. image:: ../_static/tile_size_compare.jpg
        :alt: Tile Size Comparison in Eevee.

* **Volumetric Samples**: This controls the number of times that Eevee calculates a render pass for the volume in the nebula.
* **Volumetric Shadow Samples**: This controls the number of times that Eevee calculates the quality of the shadows when doing a render pass.
* **Bloom Threshold**: This affects the glow of the stars.  Reducing this value increases the number of stars affected and the overall brightness of the nebula.
* **Bloom Intensity**: How blended with the image the bloom effect is. Lower values will reduce the overall effect.

Cycles Quality Settings
------------------------------------

.. image:: ../_static/cycles_quality_settings.jpg
    :alt: Cycles Quality Settings
    
Samples
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The number of times Cycles will calculate a render pass.  Higher levels will increase details, but will also increase time to render and system usage.

.. image:: ../_static/samples_compare.jpg
    :alt: Samples comparison


* **Viewport Samples**: The number of times Cycles will calculate a render pass in the viewport. 
* **Render Samples**: The number of times Cycles will calculate a render pass at render time. 


Denoising
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

|Denoising| is automatically switched on whilst rendering to remove |fireflies|, or speckles, in the nebula effect.  Sometimes, this may produce a slightly *liquid* effect at lower sample settings.  You may wish to turn the denoiser off and increase the sample settings in this case.

* **Denoiser**:  Which denoising function to use. Using this combined with the *samples* settings should produce a smoother result.  

.. image:: ../_static/denoising_compare.jpg
    :alt: Denoising comparison

.. |Denoising| raw:: html
    
   <a href="https://docs.blender.org/manual/en/latest/render/layers/denoising.html" target="_blank"><b>Denoising</b></a>


Step Rate
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This essentially controls the 'thickness' of the nebula volume in the viewport, or in other words the distance between points in the volume. Lower values increase the thickness.

    .. image:: ../_static/step_rate_compare.jpg
        :alt: Step Rate Comparison

* **Viewport Step Rate**:  The 'thickness' of the nebula volume in the viewport.
* **Render Step Rate**: The 'thickness' of the nebula volume in the viewport at render time.


Glare Threshold and Mix
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This controls the amount of post-processing *Glare* is added to the render, which affects star glow. 

* **Threshold**:  Increasing this parameter will make the stars and image glow less.
* **Mix**: This controls how much the glare effect is mixed witht the final image: 0.0 represets 50% Glare, -1 will remove the Glare and +1 will overwrite the image with the Glare effect.

.. |fireflies| raw:: html
    
   <a href="https://www.blenderguru.com/articles/7-ways-get-rid-fireflies" target="_blank"><b>Fireflies</b></a>