# climada-coding-conventions

## Use your notebook tutorial as a slideshow

You can convert any notebook to a HTML-based slideshow using the following command line:

    jupyter nbconvert --to slides path/to/your_notebook.ipynb

However, for the result to be useful, you have to manually mark the cells that are at the begin of each new slide:
 
* When you are in `jupyter notebook` (as opposed to `jupyter lab`), select `View -> Cell Toolbar -> Slideshow` from the menu. Now you can select a "Slide Type" in the top right corner of each cell.
* When you are in `jupyter lab`, you can change the cell type using the "Property Inspector" on the left (gear wheels symbol).
 
As a "Slide Type", use "Slide", "Sub-Slide" or "Fragment". Leave the type empty for cells that should be grouped together with the previous cell. Choose "Skip" and "Notes" for cells that shouldn't be included in your slideshow.

Run the `nbconvert`-command from above and open the new `.html` file in a browser. You can navigate using the arrow keys on your keyboard or by clicking on the arrows in the bottom right corner. "Sub-Slides" are accessed using the down arrow. On each slide, "Fragments" only appear after pressing either the down or right arrow.
