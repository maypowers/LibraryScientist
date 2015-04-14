# LibraryScientist

###sierraholds.py
Requesting a list of outstanding holds from iii Sierra generates either a printable list or a "print to email" list. Having this in a spreadsheet would be more useful, but Sierra seems unable to create a csv version of the list of outstanding holds.

sierraholds.py will generate a .csv from a .txt list of outstanding holds. It removes page numbering ("Page x") and splits out patron info (name, patron number, email, phone) by line.

Latest version:
- Hard code input file as "mail.google.com" (should be default file name when saving from mail client, though not universal across browsers). Script now runs on that filename in current directory. Comment out command line argument bits in case we want to put them back later.
- Change command line usage to 'python sierraholds.py'.
- Handle header from file as saved from mail client (i.e. remove mail header and report header).
- Output to file containing hold report timestamp.
