------------------------------------------------
Title: Universiti Malaya Unofficial Lab Report Template
Author: Errol Tay
------------------------------------------------

Hello, this is my first ever template. It took a while to make this, so I hope you enjoy using it! Read through this file to understand how stuff were implemented, and feel free to modify any part and share it.

This template was heavily inspired by Rahul Raoniar, author of "IIT Bombay Unofficial Lab Report LaTeX Format". I have modified this template to fit the lab report requirements of Universiti Malaya, Department of Physics.

---------------------

This template consists of : 
    - Four main folders, 
    - One ref.bib file, and 
    - One main.tex file.

---------------------

---------------------
A. Four Main Folders 
---------------------

1. `Appendix`
Consists of three files :

> A1. Calculations.tex: Tedious calculations are shown here, per the rules of our lab.

> A2. Gallery.tex: Any images relating to the experiment can be displayed here.

> A3. Code.tex: Python code for data analysis is displayed in IPython style.


------------------------
2. `Figures`
Consists of two directories :

> exp : Contains all experiment related images (add graphs and pictures here).

> Logo : Contains only Univeristy related images (no need to edit).


------------------------
3. `General`
Consists of the following files :

> customcommands.tex: These commands are those that are called frequently within the report itself. Three main sections :
    - Lab Specific Commands
    - General Command
    - Tcolorboxes design
    
*IMPORTANT: 
THESE ARE NOT COMMANDS THAT MODIFY STYLES, COLOR & LOOKS OF THE REPORT (that would be settings.tex).

> headerfooter.tex: There are only two header footer style used in this template. Two commands :
    - reportContent
    - reportMinimalist

> preamble.tex: All packages are here. There 26 packages used for now.

> settings.tex: Customisation of report number, report title, student name, matric number, lecturers, date, colour, font, etc... :

*IMPORTANT: 
- Contains all commands related to the documents style, colour and looks (customize every aspect of the lab report).


------------------------
4. `Sections`
The `Sections` folder consists of nine files :-

0. Frontpage.tex
1. Objectives.tex
2. Instruments.tex
3. Introduction.tex
4. Procedure.tex
5. Results.tex
6. Discussion.tex
7. Conclusion.tex
8. References.tex: (Automatic, no need edit anything).

---------------------
B. ref.bib file 
---------------------

Uses biblatex. To change \cite{} style, change settings in \General\preamble.tex. Also, I have compiled some common types of citation for easy use.

---------------------
C. main.tex file 
---------------------

The main file calls all the .tex files to be loaded. Importantly, it MUST CALL THESE 4 FILES IN THIS ORDER: 

preamble.tex -> settings.tex -> customcommands -> headerfooter 
