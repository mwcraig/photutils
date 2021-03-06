0.2 (unreleased)
----------------

General
^^^^^^^

- photutils now requires AstroPy v1.0 or later.
- photutils now requires python 2.7 or 3.3 or later.

New Features
^^^^^^^^^^^^

- ``photutils.aperture_photometry``

  - Fixed an issue where ``np.nan`` or ``np.inf`` were not properly
    masked. [#267]

- ``photutils.detection``

  - ``find_peaks`` now returns an Astropy Table containing the (x, y)
    positions and peak values. [#240]

  - ``find_peaks`` has new ``mask``, ``error``, ``wcs`` and ``subpixel``
    precision options. [#244]

- ``photutils.morphology``

  - Added new ``GaussianConst2D`` (2D Gaussian plus a constant) model
    [#244].

  - Added new ``marginalize_data2d`` function [#244].

  - Added new ``cutout_footprint`` function [#244].

Bug Fixes
^^^^^^^^^

- ``photutils.geometry``

  - ``overlap_area_triangle_unit_circle`` handles correctly a corner case
    in some i386 systems where the area of the aperture was not computed
    correctly. [#242]

  - ``rectangular_overlap_grid`` and ``elliptical_overlap_grid`` fixes to
    normalization of subsampled pixels. [#265]

  - ``overlap_area_triangle_unit_circle`` handles correctly the case where
    a line segment intersects at a triangle vertex. [#277]

Other Changes and Additions
^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Update astropy-helpers to v1.0.5 [#286]


0.1 (December 22, 2014)
-----------------------

photutils 0.1 was released on December 22, 2014.
It requires Astropy version 0.4 or later.

