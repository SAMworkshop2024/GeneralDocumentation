# General Documentation
This is a high-level repository to connect and discribe the general use of repositories within this organisation.

- [code](https://github.com/SAMworkshop2024/code): This is the main working repository. Will do the bulk if not all of the work.
- [aostools](https://github.com/SAMworkshop2024/aostools): includes hopefully useful postprocessing code. All functions are in [aostools.climate](https://github.com/SAMworkshop2024/aostools/climate.py). Useful functions could be:
    - `ClimateIndex()`: Can be used to compute flavors of ENSO, IOD, and SAM. Note that this function has not been benchmarked against other methods or functions. While care has been taken to try and follow best practices such as UCAR climatedata guidance, there might always be bugs.
    - `Projection()`: Create a cartopy-enabled figure with one or several panels. Tries to make it easier to plot data on maps.
