# General Documentation
This is a high-level repository to connect and discribe the general use of repositories within this organisation.

## Repository descriptions

- [code](https://github.com/SAMworkshop2024/code): This is the main working repository. Will do the bulk if not all of the work.
- [ESMValTool](https://github.com/SAMworkshop2024/ESMValTool): This is designated to become a standard for climate analyses. Too complicated for me (mxj), but maybe helpful to others.
- [aostools](https://github.com/SAMworkshop2024/aostools): includes hopefully useful postprocessing code. All functions are in [aostools.climate](https://github.com/SAMworkshop2024/aostools/climate.py). Useful functions could be:
    - `ClimateIndex()`: Can be used to compute flavors of ENSO, IOD, and SAM. Note that this function has not been benchmarked against other methods or functions. While care has been taken to try and follow best practices such as UCAR climatedata guidance, there might always be bugs.
    - `StatTest()`: Perform various standard statistical significance tests. This can be run in parallel.
    - `Anomaly()`: Compute an anomaly without having to type .groupby(time.dayofyear) or similar all the time.
    - `Standardize()`: Similar but also divide by standard deviation.
    - `Projection()`: Create a cartopy-enabled figure with one or several panels. Tries to make it easier to plot data on maps.
    - `StandardGrid()`: Rename longitude,latitude,pressure to 'lon','lat','pres' and make sure latitude is from -90 to 90 and longitude from 0 to 360.
    - `AddPanelLabels()`: Adds a),b),c)... labels to multi-panel figures.
    - `AddColorbar()`: Adds one common colorbar to a figure with multiple panels.
    - `LogPlot()`: Transforms the y-axis from linear into inverted log (of course, this is with pressure coordinates in mind). Also transforms axis labels to something more legible.
    - and loads more....

 ## Best practice

 1. Every user creates their own branch of a given repository and merges finished, debugged code back into the main branch via Pull Requests.
 2. Try to minimise code duplication. Re-using once might be acceptable, twice is too much. Create a function for a task which is re-used more than once. I suggest adding a file called `functions.py` which will contain such functions.
 3. Existing code is welcome, and one can build on it. Otherwise, we go back to point 2., and honestly, who ever wants to go back to point 2.?
    
## Documentation
- [CLEX CMS git tutorial](https://youtu.be/Z7kMhD0QiZE?si=zC6QX37saQZv9_Dn)
- [GitHub Docs](https://docs.github.com/en) and [getting started](https://docs.github.com/en/get-started)
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
