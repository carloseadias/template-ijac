======================================================================
COMPILATION AND USAGE INSTRUCTIONS FOR THE IJAC TEMPLATE
======================================================================

1. PROJECT STRUCTURE
This project has been split into multiple files to facilitate the 
organization and writing of your paper.

- The file "000.main_ijac.tex" is the MAIN FILE. 
  Usually, **YOU SHOULD NOT EDIT IT**, unless you need to add new 
  packages (usepackage) or include/remove chapters (extra .tex files).
- The other files (001, 002, 101, 102...) contain the content of 
  the article. Edit them to write your text.

2. ABNTEX2 FILES
To keep things organized, the abntex2 files must be placed inside the 
"abntex2" folder. The base file is already configured to pull them 
from there.

3. HOW TO COMPILE
Below are the instructions to compile the document in different 
environments:

>>> A. OVERLEAF
1. Create a new blank project in Overleaf.
2. Upload the ZIP file directly to the project.
3. Open the "000.main_ijac.tex" file and click the green "Recompile" 
   button. Overleaf will handle BibTeX processing automatically.

>>> B. MIKTEX / TEXWORKS
1. Extract all contents of the ZIP into a folder on your computer.
2. Open the "000.main_ijac.tex" file using TeXworks.
3. In the top-left dropdown menu, make sure "pdfLaTeX" is selected.
4. Click the green Play button (or press Ctrl+T) to compile.
5. Change the dropdown menu from "pdfLaTeX" to "BibTeX" and click 
   Play again. (This prepares the references).
6. Change it back to "pdfLaTeX" and click Play two more times. 
   This ensures that all cross-references and citations are properly 
   updated.

>>> C. TERMINAL / COMMAND LINE
Run the following sequence:
Step 1: pdflatex 000.main_ijac.tex
Step 2: bibtex 000.main_ijac
Step 3: pdflatex 000.main_ijac.tex
Step 4: pdflatex 000.main_ijac.tex
