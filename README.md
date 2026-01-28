#Fork and branch specifics
This is a fork from gfdl/dev, with ice thermodynamics altered to include a simple ghost flux over sea ice. This branch is at a commit state compareble with mom6-panan. The ghost flux is assigned at the namelist level, and applied globally, only constrained by latitude indexes. Edits in SIS2 code made by Wilton Aguiar


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
