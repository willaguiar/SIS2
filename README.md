# Ghost Flux
This is a fork from gfdl/dev, with ice thermodynamics altered to include a simple longwave ghost flux over sea ice. This branch is at a commit state compatible with  mom6-panan and can be used directly for compilation of panan. The ghost flux is assigned as a set of parameters under SIS_input in panan, and applied circumpolarlly, only constrained by latitude indexes. The relevant parameters for the ghost flux are:

`GHOST_LW_ICE_ON` : if True, applies the ghost flux. default = False


`GHOST_LW_ICE` : Ghost longwave flux applied to ice thermodynamics (W m-2). default = 0.0


`GHOST_LW_LAT_SOUTH` : Southern ghost flux boundary in degrees. default=-90, i.e., 90S


`GHOST_LW_LAT_NORTH` : Northern ghost flux boundary in degrees. default = -40, i.e., 40S


As you can see, this is a rather simplistic ghost flux application, as it applies a "geographically rectangular" longwave ghost flux. That means that if the prescribed flux is too big you might end up with a unphysical square ice border. So try to apply reasonably high, but not unphysically high ghost flux values


by Wilton Aguiar


# SIS2

NOAA-GFDL's Sea Ice Simulator version 2

# Disclaimer

The United States Department of Commerce (DOC) GitHub project code is provided
on an "as is" basis and the user assumes responsibility for its use. DOC has
relinquished control of the information and no longer has responsibility to
protect the integrity, confidentiality, or availability of the information. Any
claims against the Department of Commerce stemming from the use of its GitHub
project will be governed by all applicable Federal law. Any reference to
specific commercial products, processes, or services by service mark,
trademark, manufacturer, or otherwise, does not constitute or imply their
endorsement, recommendation or favoring by the Department of Commerce. The
Department of Commerce seal and logo, or the seal and logo of a DOC bureau,
shall not be used in any manner to imply endorsement of any commercial product
or activity by DOC or the United States Government.

This project code is made available through GitHub but is managed by NOAA-GFDL
at https://gitlab.gfdl.noaa.gov.
