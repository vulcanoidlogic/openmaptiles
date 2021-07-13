## Quickstart - for small extracts

### Req:
* CPU: AMD64 ( = Intel 64 bit)
    *  The base docker debian images are x86_64 based, so the ARM,MIPS currently not supported!
* Operating system
    * Linux is suggested
        * The development and the testing platform is Linux.
    * If you are using FreeBSD, Solaris, Windows, ...
        * Please give a feedback, share your experience, write a tutorial
* bash
* git
* make
* bc
* md5sum
* docker         >=1.12.3
    * https://www.docker.com/products/overview
* docker-compose >=1.7.1
    * https://docs.docker.com/compose/install/
* disk space ( >= ~15Gb  )
    * for small extracts  >= ~15Gb
    * for big extracts ( continents, planet) 250 Gb
    * And depends on
        * OpenStreetMap data size
        * Zoom level
    * Best on SSD for postserve but completely usable on HDD
    * Takes 24hrs to import on a reasonable machine, and is immediately available with postserve
* memory ( >= 3Gb )
    * for small extracts 3Gb-8Gb RAM
    * for big extracts ( Europe, Planet) > 8-32 Gb
* internet connections
    * for downloading docker images
    * for downloading OpenStreetMap data from Geofabrik

Important:  The ./init.sh is for small extracts - not optimal for a Planet rendering !!

### First experiment - with `albania` ( small extracts! )

```bash
git clone https://github.com/openmaptiles/openmaptiles.git
cd openmaptiles
./init.sh
```

If you have problems with the quickstart
* check the ./quickstart.log!
* doublecheck the system requirements!
* check the current issues: https://github.com/openmaptiles/openmaptiles/issues
* create new issues:
    * create a new gist: https://gist.github.com/ from your ./quickstart.log
    * doublecheck: don't reveal any sensitive information about your system
    * create a new issue: https://github.com/openmaptiles/openmaptiles/issues
        * describe the problems
        * add any pertinent information about your environment
        * link your (quickstart.log) gist!

### Check other extracts

IF the previous step is working,
THEN you can test other available quickstart extracts ( based on [Geofabrik extracts](http://download.geofabrik.de/index.html) ) !
 * We are using https://github.com/julien-noblet/download-geofabrik tool
 * The current extract list, and more information  ->  `make list`

This is generating `.mbtiles` for your area :  [ MIN_ZOOM: "0"  - MAX_ZOOM: "7" ]

```bash
./init.sh africa                       # Africa
./init.sh alabama                      # Alabama, US
./init.sh alaska                       # Alaska, US
./init.sh albania                      # Albania, Europe
./init.sh alberta                      # Alberta, Canada
./init.sh alps                         # Alps, Europe
./init.sh alsace                       # Alsace, France
./init.sh andorra                      # Andorra, Europe
./init.sh antarctica                   # Antarctica
./init.sh aquitaine                    # Aquitaine, France
./init.sh argentina                    # Argentina, South-America
./init.sh arizona                      # Arizona, US
./init.sh arkansas                     # Arkansas, US
./init.sh arnsberg-regbez              # Regierungsbezirk Arnsberg, Nordrhein-Westfalen
./init.sh asia                         # Asia
./init.sh australia                    # Australia, Australia-Oceania
./init.sh australia-oceania            # Australia and Oceania
./init.sh austria                      # Austria, Europe
./init.sh auvergne                     # Auvergne, France
./init.sh azerbaijan                   # Azerbaijan, Asia
./init.sh azores                       # Azores, Europe
./init.sh baden-wuerttemberg           # Baden-Württemberg, Germany
./init.sh bangladesh                   # Bangladesh, Asia
./init.sh basse-normandie              # Basse-Normandie, France
./init.sh bayern                       # Bayern, Germany
./init.sh belarus                      # Belarus, Europe
./init.sh belgium                      # Belgium, Europe
./init.sh belize                       # Belize, Central-America
./init.sh berlin                       # Berlin, Germany
./init.sh bolivia                      # Bolivia, South-America
./init.sh bosnia-herzegovina           # Bosnia-Herzegovina, Europe
./init.sh botswana                     # Botswana, Africa
./init.sh bourgogne                    # Bourgogne, France
./init.sh brandenburg                  # Brandenburg, Germany
./init.sh brazil                       # Brazil, South-America
./init.sh bremen                       # Bremen, Germany
./init.sh bretagne                     # Bretagne, France
./init.sh british-columbia             # British Columbia, Canada
./init.sh british-isles                # British Isles, Europe
./init.sh buckinghamshire              # Buckinghamshire, England
./init.sh bulgaria                     # Bulgaria, Europe
./init.sh burkina-faso                 # Burkina Faso, Africa
./init.sh california                   # California, US
./init.sh cambridgeshire               # Cambridgeshire, England
./init.sh cameroon                     # Cameroon
./init.sh canada                       # Canada, North-America
./init.sh canary-islands               # Canary Islands, Africa
./init.sh central-america              # Central America
./init.sh centre                       # Centre, France
./init.sh champagne-ardenne            # Champagne Ardenne, France
./init.sh cheshire                     # Cheshire, England
./init.sh chile                        # Chile, South-America
./init.sh china                        # China, Asia
./init.sh colombia                     # Colombia, South-America
./init.sh colorado                     # Colorado, US
./init.sh congo-democratic-republic    # Congo (Democratic Republic), Africa
./init.sh connecticut                  # Connecticut, US
./init.sh cornwall                     # Cornwall, England
./init.sh corse                        # Corse, France
./init.sh croatia                      # Croatia, Europe
./init.sh cuba                         # Cuba, Central-America
./init.sh cumbria                      # Cumbria, England
./init.sh cyprus                       # Cyprus, Europe
./init.sh czech-republic               # Czech Republic, Europe
./init.sh dach                         # Germany, Austria, Switzerland, Europe
./init.sh delaware                     # Delaware, US
./init.sh denmark                      # Denmark, Europe
./init.sh derbyshire                   # Derbyshire, England
./init.sh detmold-regbez               # Regierungsbezirk Detmold, Nordrhein-Westfalen
./init.sh devon                        # Devon, England
./init.sh district-of-columbia         # District of Columbia, US
./init.sh dorset                       # Dorset, England
./init.sh duesseldorf-regbez           # Regierungsbezirk Düsseldorf, Nordrhein-Westfalen
./init.sh east-sussex                  # East Sussex, England
./init.sh east-yorkshire-with-hull     # East Yorkshire with Hull, England
./init.sh ecuador                      # Ecuador, South-America
./init.sh egypt                        # Egypt, Africa
./init.sh england                      # England, Great-Britain
./init.sh essex                        # Essex, England
./init.sh estonia                      # Estonia, Europe
./init.sh ethiopia                     # Ethiopia, Africa
./init.sh europe                       # Europe
./init.sh faroe-islands                # Faroe Islands, Europe
./init.sh fiji                         # Fiji, Australia-Oceania
./init.sh finland                      # Finland, Europe
./init.sh florida                      # Florida, US
./init.sh france                       # France, Europe
./init.sh franche-comte                # Franche Comte, France
./init.sh freiburg-regbez              # Regierungsbezirk Freiburg, Baden-Wuerttemberg
./init.sh gcc-states                   # GCC States, Asia
./init.sh georgia-eu                   # Georgia (Eastern Europe), Europe
./init.sh georgia-us                   # Georgia (US State), US
./init.sh germany                      # Germany, Europe
./init.sh gloucestershire              # Gloucestershire, England
./init.sh great-britain                # Great Britain, Europe
./init.sh greater-london               # Greater London, England
./init.sh greater-manchester           # Greater Manchester, England
./init.sh greece                       # Greece, Europe
./init.sh greenland                    # Greenland, North-America
./init.sh guadeloupe                   # Guadeloupe, France
./init.sh guatemala                    # Guatemala, Central-America
./init.sh guinea                       # Guinea, Africa
./init.sh guinea-bissau                # Guinea-Bissau, Africa
./init.sh guyane                       # Guyane, France
./init.sh haiti-and-domrep             # Haiti and Dominican Republic, Central-America
./init.sh hamburg                      # Hamburg, Germany
./init.sh hampshire                    # Hampshire, England
./init.sh haute-normandie              # Haute-Normandie, France
./init.sh hawaii                       # Hawaii, US
./init.sh herefordshire                # Herefordshire, England
./init.sh hertfordshire                # Hertfordshire, England
./init.sh hessen                       # Hessen, Germany
./init.sh hungary                      # Hungary, Europe
./init.sh iceland                      # Iceland, Europe
./init.sh idaho                        # Idaho, US
./init.sh ile-de-france                # Ile-de-France, France
./init.sh illinois                     # Illinois, US
./init.sh india                        # India, Asia
./init.sh indiana                      # Indiana, US
./init.sh indonesia                    # Indonesia, Asia
./init.sh iowa                         # Iowa, US
./init.sh irak                         # Irak, Asia
./init.sh iran                         # Iran, Asia
./init.sh ireland-and-northern-ireland # Ireland and Northern Ireland, Europe
./init.sh isle-of-man                  # Isle of Man, Europe
./init.sh isle-of-wight                # Isle of Wight, England
./init.sh israel-and-palestine         # Israel and Palestine, Asia
./init.sh italy                        # Italy, Europe
./init.sh ivory-coast                  # Ivory Coast, Africa
./init.sh japan                        # Japan, Asia
./init.sh jordan                       # Jordan, Asia
./init.sh kansas                       # Kansas, US
./init.sh karlsruhe-regbez             # Regierungsbezirk Karlsruhe, Baden-Wuerttemberg
./init.sh kazakhstan                   # Kazakhstan, Asia
./init.sh kent                         # Kent, England
./init.sh kentucky                     # Kentucky, US
./init.sh kenya                        # Kenya, Africa
./init.sh koeln-regbez                 # Regierungsbezirk Köln, Nordrhein-Westfalen
./init.sh kosovo                       # Kosovo, Europe
./init.sh kyrgyzstan                   # Kyrgyzstan, Asia
./init.sh lancashire                   # Lancashire, England
./init.sh languedoc-roussillon         # Languedoc-Roussillon, France
./init.sh latvia                       # Latvia, Europe
./init.sh lebanon                      # Lebanon, Asia
./init.sh leicestershire               # Leicestershire, England
./init.sh lesotho                      # Lesotho, Africa
./init.sh liberia                      # Liberia, Africa
./init.sh libya                        # Libya, Africa
./init.sh liechtenstein                # Liechtenstein, Europe
./init.sh limousin                     # Limousin, France
./init.sh lithuania                    # Lithuania, Europe
./init.sh lorraine                     # Lorraine, France
./init.sh louisiana                    # Louisiana, US
./init.sh luxembourg                   # Luxembourg, Europe
./init.sh macedonia                    # Macedonia, Europe
./init.sh madagascar                   # Madagascar, Africa
./init.sh maine                        # Maine, US
./init.sh malaysia-singapore-brunei    # Malaysia, Singapore, and Brunei, Asia
./init.sh malta                        # Malta, Europe
./init.sh manitoba                     # Manitoba, Canada
./init.sh martinique                   # Martinique, France
./init.sh maryland                     # Maryland, US
./init.sh massachusetts                # Massachusetts, US
./init.sh mayotte                      # Mayotte, France
./init.sh mecklenburg-vorpommern       # Mecklenburg-Vorpommern, Germany
./init.sh mexico                       # Mexico, North-America
./init.sh michigan                     # Michigan, US
./init.sh midi-pyrenees                # Midi-Pyrenees, France
./init.sh minnesota                    # Minnesota, US
./init.sh mississippi                  # Mississippi, US
./init.sh missouri                     # Missouri, US
./init.sh mittelfranken                # Mittelfranken, Bayern
./init.sh moldova                      # Moldova, Europe
./init.sh monaco                       # Monaco, Europe
./init.sh mongolia                     # Mongolia, Asia
./init.sh montana                      # Montana, US
./init.sh montenegro                   # Montenegro, Europe
./init.sh morocco                      # Morocco, Africa
./init.sh muenster-regbez              # Regierungsbezirk Münster, Nordrhein-Westfalen
./init.sh nebraska                     # Nebraska, US
./init.sh nepal                        # Nepal, Asia
./init.sh netherlands                  # Netherlands, Europe
./init.sh nevada                       # Nevada, US
./init.sh new-brunswick                # New Brunswick, Canada
./init.sh new-caledonia                # New Caledonia, Australia-Oceania
./init.sh new-hampshire                # New Hampshire, US
./init.sh new-jersey                   # New Jersey, US
./init.sh new-mexico                   # New Mexico, US
./init.sh new-york                     # New York, US
./init.sh new-zealand                  # New Zealand, Australia-Oceania
./init.sh newfoundland-and-labrador    # Newfoundland and Labrador, Canada
./init.sh niederbayern                 # Niederbayern, Bayern
./init.sh niedersachsen                # Niedersachsen, Germany
./init.sh nigeria                      # Nigeria, Africa
./init.sh nord-pas-de-calais           # Nord-Pas-de-Calais, France
./init.sh nordrhein-westfalen          # Nordrhein-Westfalen, Germany
./init.sh norfolk                      # Norfolk, England
./init.sh north-america                # North America
./init.sh north-carolina               # North Carolina, US
./init.sh north-dakota                 # North Dakota, US
./init.sh north-korea                  # North Korea, Asia
./init.sh north-yorkshire              # North Yorkshire, England
./init.sh northwest-territories        # Northwest Territories, Canada
./init.sh norway                       # Norway, Europe
./init.sh nottinghamshire              # Nottinghamshire, England
./init.sh nova-scotia                  # Nova Scotia, Canada
./init.sh nunavut                      # Nunavut, Canada
./init.sh oberbayern                   # Oberbayern, Bayern
./init.sh oberfranken                  # Oberfranken, Bayern
./init.sh oberpfalz                    # Oberpfalz, Bayern
./init.sh ohio                         # Ohio, US
./init.sh oklahoma                     # Oklahoma, US
./init.sh ontario                      # Ontario, Canada
./init.sh oregon                       # Oregon, US
./init.sh oxfordshire                  # Oxfordshire, England
./init.sh pakistan                     # Pakistan, Asia
./init.sh paraguay                     # Paraguay, South-America
./init.sh pays-de-la-loire             # Pays de la Loire, France
./init.sh pennsylvania                 # Pennsylvania, US
./init.sh peru                         # Peru, South-America
./init.sh philippines                  # Philippines, Asia
./init.sh picardie                     # Picardie, France
./init.sh poitou-charentes             # Poitou-Charentes, France
./init.sh poland                       # Poland, Europe
./init.sh portugal                     # Portugal, Europe
./init.sh prince-edward-island         # Prince Edward Island, Canada
./init.sh provence-alpes-cote-d-azur   # Provence Alpes-Cote-d'Azur, France
./init.sh quebec                       # Quebec, Canada
./init.sh reunion                      # Reunion, France
./init.sh rheinland-pfalz              # Rheinland-Pfalz, Germany
./init.sh rhode-island                 # Rhode Island, US
./init.sh rhone-alpes                  # Rhone-Alpes, France
./init.sh romania                      # Romania, Europe
./init.sh russia-asian-part            # Russia (Asian part), Asia
./init.sh russia-european-part         # Russia (European part), Europe
./init.sh saarland                     # Saarland, Germany
./init.sh sachsen                      # Sachsen, Germany
./init.sh sachsen-anhalt               # Sachsen-Anhalt, Germany
./init.sh saskatchewan                 # Saskatchewan, Canada
./init.sh schleswig-holstein           # Schleswig-Holstein, Germany
./init.sh schwaben                     # Schwaben, Bayern
./init.sh scotland                     # Scotland, Great-Britain
./init.sh serbia                       # Serbia, Europe
./init.sh shropshire                   # Shropshire, England
./init.sh sierra-leone                 # Sierra Leone, Africa
./init.sh slovakia                     # Slovakia, Europe
./init.sh slovenia                     # Slovenia, Europe
./init.sh somalia                      # Somalia, Africa
./init.sh somerset                     # Somerset, England
./init.sh south-africa-and-lesotho     # South Africa (includes Lesotho), Africa
./init.sh south-america                # South America
./init.sh south-carolina               # South Carolina, US
./init.sh south-dakota                 # South Dakota, US
./init.sh south-korea                  # South Korea, Asia
./init.sh south-yorkshire              # South Yorkshire, England
./init.sh spain                        # Spain, Europe
./init.sh sri-lanka                    # Sri Lanka, Asia
./init.sh staffordshire                # Staffordshire, England
./init.sh stuttgart-regbez             # Regierungsbezirk Stuttgart, Baden-Wuerttemberg
./init.sh suffolk                      # Suffolk, England
./init.sh surrey                       # Surrey, England
./init.sh sweden                       # Sweden, Europe
./init.sh switzerland                  # Switzerland, Europe
./init.sh syria                        # Syria, Asia
./init.sh taiwan                       # Taiwan, Asia
./init.sh tajikistan                   # Tajikistan, Asia
./init.sh tanzania                     # Tanzania, Africa
./init.sh tennessee                    # Tennessee, US
./init.sh texas                        # Texas, US
./init.sh thailand                     # Thailand, Asia
./init.sh thueringen                   # Thüringen, Germany
./init.sh tuebingen-regbez             # Regierungsbezirk Tübingen, Baden-Wuerttemberg
./init.sh turkey                       # Turkey, Europe
./init.sh turkmenistan                 # Turkmenistan, Asia
./init.sh ukraine                      # Ukraine, Europe
./init.sh unterfranken                 # Unterfranken, Bayern
./init.sh uruguay                      # Uruguay, South-America
./init.sh us-midwest                   # US Midwest, North-America
./init.sh us-northeast                 # US Northeast, North-America
./init.sh us-pacific                   # US Pacific, North-America
./init.sh us-south                     # US South, North-America
./init.sh us-west                      # US West, North-America
./init.sh utah                         # Utah, US
./init.sh uzbekistan                   # Uzbekistan, Asia
./init.sh vermont                      # Vermont, US
./init.sh vietnam                      # Vietnam, Asia
./init.sh virginia                     # Virginia, US
./init.sh wales                        # Wales, Great-Britain
./init.sh washington                   # Washington, US
./init.sh west-midlands                # West Midlands, England
./init.sh west-sussex                  # West Sussex, England
./init.sh west-virginia                # West Virginia, US
./init.sh west-yorkshire               # West Yorkshire, England
./init.sh wiltshire                    # Wiltshire, England
./init.sh wisconsin                    # Wisconsin, US
./init.sh wyoming                      # Wyoming, US
./init.sh yukon                        # Yukon, Canada
```
### Using your own OSM data
Mbtiles can be generated from an arbitrary osm.pbf (e.g. for a region that is not covered by an existing extract) by making the `data/` directory and placing an *.osm.pbf (e.g. `mydata.osm.pbf`) inside.

```
mkdir -p data
mv mydata.osm.pbf data/
make generate-bbox-file area=mydata
./init.sh mydata
```

### Check postserve
*  ` docker-compose up -d postserve`
and the generated maps are going to be available in browser on [localhost:8090/tiles/0/0/0.pbf](http://localhost:8090/tiles/0/0/0.pbf).

### Check tileserver

start:
*  ` make start-tileserver`
and the generated maps are going to be available in webbrowser on [localhost:8080](http://localhost:8080/).

This is only a quick preview, because your mbtiles only generated to zoom level 7 !


### Set which zooms to generate

modify the settings in the `.env` file, the defaults:
* `MIN_ZOOM=0`
* `MAX_ZOOM=7`

Hints:
* Small increments! Never starts with the `MAX_ZOOM = 14`
* The suggested  `MAX_ZOOM = 14`  - use only with small extracts

### Set the bounding box to generate

By default, tile generation is done for the full extent of the area.
If you want to generate a tiles for a smaller extent, modify the settings in the `.env` file, the default:
* `BBOX=-180.0,-85.0511,180.0,85.0511`

Delete the `./data/<area>.bbox` file, and re-start `./init.sh <area>`

Hint:
* The [boundingbox.klokantech.com](https://boundingbox.klokantech.com/) site can be used to find a bounding box (CSV format) using a map.

### Check other commands

`make help`


the current output:

```
==============================================================================
 OpenMapTiles  https://github.com/openmaptiles/openmaptiles
Hints for testing areas
  make download-geofabrik-list         # list actual geofabrik OSM extracts for download -> <<your-area>>
  ./init.sh <<your-area>>        # example:  ./init.sh madagascar

Hints for designers:
  make start-postserve                 # start Postserver + Maputnik Editor [ see localhost:8088 ]
  make start-tileserver                # start maptiler/tileserver-gl [ see localhost:8080 ]

Hints for developers:
  make                                 # build source code
  make download-geofabrik area=albania # download OSM data from geofabrik, and create config file
  make psql                            # start PostgreSQL console
  make psql-list-tables                # list all PostgreSQL tables
  make psql-vacuum-analyze             # PostgreSQL: VACUUM ANALYZE
  make psql-analyze                    # PostgreSQL: ANALYZE
  make generate-qa                     # statistics for a given layer's field
  make generate-devdoc                 # generate devdoc  [./build/devdoc]
  make tools-dev                       # start import-sql  /bin/bash terminal
  make db-destroy                      # remove docker containers, PG data volume
  make docker-unnecessary-clean        # clean unnecessary docker image(s) and container(s)
  make refresh-docker-images           # refresh openmaptiles docker images from Docker HUB
  make remove-docker-images            # remove openmaptiles docker images
  make list-views                      # list PostgreSQL public schema views
  make list-tables                     # list PostgreSQL public schema tables
  cat  .env                            # list PG database and MIN_ZOOM and MAX_ZOOM information
  cat ./quickstart.log                 # backup  of the last ./init.sh
  make help                            # help about available commands
==============================================================================
```
