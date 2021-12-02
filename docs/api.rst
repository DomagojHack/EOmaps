⚙ API
=======

🔸 Initialize Maps objects
----------------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps.Maps
    eomaps.Maps.copy
    eomaps.MapsGrid


🔸 Set specifications
-----------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps.Maps.set_shape
    eomaps.Maps.set_data
    eomaps.Maps.set_data_specs
    eomaps.Maps.set_plot_specs
    eomaps.Maps.set_classify_specs


You can also get/set the specs with:

.. code-block:: python

    eomaps.Maps.data_specs.<...name...>
    eomaps.Maps.plot_specs.<...name...>
    eomaps.Maps.classify_specs.<...name...>


🔸 Plot the map and save it
-----------------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps.Maps.plot_map
    eomaps.Maps.savefig

    eomaps.Maps.figure


🔸 Add layers and objects
---------------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps.Maps.add_wms
    eomaps.Maps.add_wmts
    eomaps.Maps.add_gdf
    eomaps.Maps.add_overlay
    eomaps.Maps.add_overlay_legend
    eomaps.Maps.add_coastlines

    eomaps.Maps.add_marker
    eomaps.Maps.add_annotation
    eomaps.Maps.add_colorbar


🔸 Miscellaneous
------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps.Maps.get_crs
    eomaps.Maps.CRS
    eomaps.Maps.CLASSIFIERS
    eomaps.Maps.indicate_masked_points
    eomaps.Maps.parent
    eomaps.Maps.BM
    eomaps.Maps.crs_plot
    eomaps.Maps.join_limits

🔸 Add Callbacks
------------------

.. autosummary::
    :toctree: generated
    :nosignatures:

    eomaps._cb_container.cb_container
    eomaps._cb_container.cb_container.click
    eomaps._cb_container.cb_container.pick
    eomaps._cb_container.cb_container.keypress
    eomaps._cb_container.cb_container.dynamic


🔸 Pre-defined callbacks
--------------------------

.. currentmodule:: eomaps.callbacks._click_callbacks

Click & pick callbacks
......................

Callback functions usable with both `m.cb.click` and `m.cb.pick`:

.. autosummary::
    :toctree: generated
    :nosignatures:
    :template: function_onlynames.rst

    peek_layer
    annotate
    clear_annotations
    mark
    clear_markers
    get_values
    print_to_console

Callbacks usable only with `m.cb.pick`:

.. autosummary::
    :toctree: generated
    :nosignatures:
    :template: function_onlynames.rst

    load

Keypress callbacks
..................

.. currentmodule:: eomaps.callbacks.keypress_callbacks

.. autosummary::
    :toctree: generated
    :nosignatures:
    :template: function_onlynames.rst

    switch_layer

Dynamic callbacks
..................

.. currentmodule:: eomaps.callbacks.dynamic_callbacks

.. autosummary::
    :toctree: generated
    :nosignatures:
    :template: function_onlynames.rst

    indicate_extent
