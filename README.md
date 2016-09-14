# ecc-updates
ecc-updates are (small) side updates wich can include hotfixes and improvements.
eccLive! can download and install these updates to your emuControlCenter installation.
This way you won't need to download a new version of ECC everytime.

**NOTE: This is only for TAGGED releases, releases in the repository are up-to-date!**

LAST UPDATES:

----- ECC v1.21 -----

Update 00622 2016-09-14
- CORE
  - Added 3 new metadata fields to ECC database and GUI, also being exported from and imported to ECC.
    - Perspective, Visual, Description
  - Some Code and GUI cleanup.
  - Mobygames
    - v1.2.0.0
      - Added new fields to fill Perspective, Visual
      - Description now in the META data location (instead of userdata)
  - ECC Tool variables
      - v1.0.0.8
        - Fixed an issue where the database could not be found at the "default" location.

Update 00621 2016-09-03
- CORE
  - Fixed link to TAB help on mainscreen to readme.md.
  - Manager: ecccli_datFileImporter.php, Fixed database fixed location, now reading ecc settings.
  - Fixed and added function to start SQlite browser without the autoit3 script!
- ECC Startup
  - v3.0.0.2
    - Using animated GIF instead of AVI for loading animations, you can make you own easily now!
      You can find instructions at emuControlCenter WIKI on GitHub.
- ECC Tool variables
  - v1.0.0.1
    - Added new variables for eccdb, now reading ecc settings.
- SOURCE
  - Added new resource file "ecc_splashscreen_borders.psd" this is a reworked splashscreen combination.
- THEMES
  - Added loading aimation for theme: afterhours, miss-kit-purple
  - Removed incomplete themes: miss-kit-bubblegum, green-grass, nature-full-green
    (Only on fresh installations)

Update 00620 2016-09-02
- CORE
  - Reworked configuration GUI, placed options together where needed, deleted old options and TABS.
  - Selectable ECC DATABASE path!, put your database on a central location so every computer
    in a network can run the same data!
    - Some notes setting and using the ECC DATABASE path:
      - With manual input always use a ending slash \.
      - Network paths are not listed, but you can type them manually like: \\COMPUTER\PATH\.
      - Wrong pathnames or no rights to write will reset the DB tot he default "ecc-system\database" location.
      - When configuring a location of a existing ECC configuration/database, you have to copy the database
        manually to the new location.
      - You may experience slow response form ECC when you store the datbaase on a network path.
      - ECC is not tested to run from multiple computers with the same database,
        the database could be "in use by another application" let me know if it works!
  - Added a new PHP class "ecc-system\manager\cIniFileRegular.php" to read and write INI files easily.
  - Database "empty" is now the updated version (save some scripts to be executed everytime)
  - Added some more translations to be made in the GUI.

Update 00619 2016-08-13
- CORE
  - Updated links in the GUI to the new ECC website.
  - Updated the teaser image.
- Scripts
  - Commodore Amiga: Merged the eccScript with the getgemusconfig script, placed
    the Amiga Gamebase inside the ecc-system\datfiles folder.
- ECC Startup v3.0.0.1
  - Fixed unpacking DAT files with spaces in the filenames.
- DAT files updates
  - Amiga Gamebase v1.6 to v2.0
- 3RD Party updates
  - Mplayer Redxii-SVN-r37153-4.8.2 to Redxii-SVN-r37871-4.9.3 (i686)

Update 00618 2016-08-12
- ECC SOURCE files released!, they include:
  - KODA AutoIt3 GUI's (KXF)
  - Photoshop images (PSD)
  - Fonts (TTF)
  - Scalable Vector Graphics (SVG)
  Files are in the 'ecc-source' folder.
- ECC: Adjusted all links to the new ECC homepage:
  - https://github.com/PhoenixInteractiveNL/emuControlCenter/wiki
- ECC startup: Minor GUI adjustement for removed checkbox.
- ECC DOCS
  - Placed Autoit and Xpadder docs in their respective folders now.
  - Updated Autoit3 Documentation.
- ECC 3D Gallery
  - v1.2.0.0
    - Adjusted variable to fetch the proper websitelink from toolvariables.au3
- ECC CreateStartmenuShotcuts
  - v1.0.0.4
    - Now fetching website link from toolvariables.au3
- ECC Update
  - v1.2.0.1
    - Now fetching website link from toolvariables.au3

UPDATE 00617
- Fix ecc-user folder structure in ECC, seems that empty folders are not stored
  on github with desktop GIT.
