# Numerical Modeling with Landlab

This repository contains materials for a series of three clinics on mathematical modeling and Landlab, at the 2022 CSDMS all-hands meeting.

To access the Jupyter Notebooks for these clinics, participants should have a JupyterHub account. They can follow the link below to access everything from this GitHub repo on JupyterHub.

[click here to pull this GitHub repo to JupyterHub](https://lab.openearthscape.org/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Flandlab%2Fcsdms_2022_landlab_clinics&urlpath=tree%2Fcsdms_2022_landlab_clinics%2F&branch=main)
## Session 1: The Art of Modeling: From Concept to Math with Mass Balance

Numerical models describe the world around us mathematically, allowing us to visualize changes to physical systems through both space and time. These models are essential tools for geoscientists, but writing your own model can be a daunting task.

In this clinic, we’ll develop an understanding of what numerical models are, and then we’ll delve into the math that functions as the basis for many models. Participants will learn how to apply basic conservation principles to developing equations that describe a physical system that changes through time. This workshop will expose participants to deriving differential equations, and using basic Python programming to visualize their solutions. Prior experience is not necessary (though familiarity with calculus is helpful).

### Goals

Learning objectives for this clinic include:

- Describe different uses of numerical models
- Understand how the mass or energy balance method can be used to derive a differential equation for a geo/environmental system
- Appreciate how simple finite-difference methods can be used to formulate discretized approximations of simple one-dimensional ODEs and diffusion-like PDEs

### Program

- What is computer modeling and why is it useful?
- Introduction to the mass balance method: example of a lake basin
  - Exercises in deriving a model and plotting solutions
- Finite-difference method: using forward-differencing to iterate in time 
- Mass balance with a spatial dimension: example of an evolving hillslope
  - Exercises in adding a source term and plotting equilibrium solutions
- Finite-differencing: forward-time, centered-space (FTCS) method
  - Exercise: playing with a simple 1d finite-difference hillslope evolution code
- Time-stepping and the Courant-Friedrichs-Lewy (CFL) constraint
- A quick look at extending to 2d
- (optional, if extra time) Energy balance: deriving and exploring a 1d heat diffusion equation


### Where to learn more?

#### Books

Slingerland, R., & Kump, L. (2011) *Mathematical Modeling of Earth's Dynamical Systems: A Primer.* Princeton University Press.

Press, W. H., Teukolsky, S. A., Vetterling, W. T., & Flannery, B. P. (2007) *Numerical recipes 3rd edition: The art of scientific computing.* Cambridge university press.


#### Hands-on tutorials

The *Landlab Fault Scarp* notebook tutorial presents numerical solutions to the diffusion equation for hillslope soil creep, with a 1D example that uses basic Python and NumPy code, a series of 2d examples using Landlab grids and functions, and an example that uses the Landlab `LinearDiffuser` component.


## Session 2: Introduction to Landlab

This clinic provides a brief tutorial introduction to the theory and implementation of Landlab for landscape evolution modeling. Topics include grid representation, working with data fields, and using Landlab components to create new integrated models. This clinic is intended for beginners with little to no experience using the Landlab library. Prior experience with Python programming is helpful.


## Session 3: Creating and Using Landlab Components

This clinic explores how to fully engage with the Landlab library by creating your own components. It is designed for those who already have some basic familiarity with Landlab and with scientific Python programming (registration for the “Introduction to Landlab” is recommended for those who have not already learned the basics). In this workshop we will cover an overview of object-oriented programming (OOP), and will look at several examples of existing Landlab components to understand how they are written in an OOP framework. We will write a demo component as a group, and will then move on to writing our own components in small groups.

Participants should come prepared with an idea of a process model they’d like to implement as a component. It is recommended, but not required, that participants in this workshop also register for the clinic “The Art of Modeling: From Concept to Math with Mass Balance,” in order to be equipped with an understanding of the math that will form the basis of their Landlab component.

This workshop will involve coding in Python using the CSDMS JupyterHub. If you don't already have an account, follow the instructions to sign up at: https://csdms.colorado.edu/wiki/JupyterHub.
