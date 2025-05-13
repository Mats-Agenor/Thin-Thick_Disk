# The Exponential Disk

This notebook was assembled based on the content of the book Galactic Dynamics — Binney & Tremaine, (2008). Its main purpose is to provide a didactic and computational approach to understanding the mass distribution and gravitational effects of exponential galactic disks. These models are fundamental in galactic astrophysics, particularly in modeling spiral galaxies like the Milky Way.

The notebook implements and compares two models of galactic disks:

A thin exponential disk, idealized as having zero thickness (infinitesimally thin).

A thick exponential disk, with a realistic vertical structure represented by a sech² vertical density profile.

Both models are used to compute:

The mass density profile as a function of galactocentric radius.

The gravitational potential in the midplane of the disk.

The circular velocity profile, derived from the potential.

These quantities are essential for understanding galactic rotation curves and mass distribution, and for comparing theoretical predictions with observational data.

What the Code Does
1. Define Physical Parameters
It starts by setting key physical constants and parameters:

The gravitational constant in astrophysical units.

The central surface density of the disk.

The radial scale length (Rd) and vertical scale height (z0) of the disk.

2. Thin Disk Model
The thin disk is treated as a surface density profile with exponential radial decay. The gravitational potential in the midplane is computed through an integral involving Bessel functions (as derived in Galactic Dynamics). From this potential, the circular velocity is computed using the radial derivative of the potential.

3. Thick Disk Model
The thick disk includes a vertical structure, with density falling off vertically according to a sech²(z/z₀) law. This model more accurately represents the three-dimensional structure of real galactic disks. The gravitational potential is computed numerically via a double integral over cylindrical coordinates. A small regularization term is introduced to avoid singularities in the integrand.

4. Plotting
The code generates and displays:

A plot comparing the surface density of the thin disk and the midplane volume density of the thick disk.

A plot of the gravitational potential for both disk models.

A plot of the circular velocity as a function of galactocentric radius.

Each plot is annotated with appropriate legends and units for clear interpretation.
