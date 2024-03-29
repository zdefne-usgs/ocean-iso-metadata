Examples using custom style sheet (an .xsl file needs to be placed under XSL for this to work):

**Example 1** - run071tRX

java -Xms1024m -Xmx1024m -jar ncISO-2.3.7.jar -custom true -xsl UnidataDD2MI_cur.xsl -ts https://geoport.usgs.esipfed.org/thredds/sand/usgs/Projects/BBLEH/run071tRX/catalog.xml -num 1 -depth 20 -iso true

**Example 2** - breach_matanzas

java -Xms1024m -Xmx1024m -jar ncISO-2.3.7.jar -custom true -xsl UnidataDD2MI_cur.xsl -ts https://geoport.usgs.esipfed.org/thredds/vortexfs1/usgs/Projects/breach/breach_matanzas/catalog.xml -num 1 -depth 20 -iso true

Each will create a JSON file for that run and will append messages to ncISO.log. The ISO xml are created in a locally created folder structure similar to the thredds server.  

**Note (01/24/2022)**

Currently there seems to be a problem with standalone ncISO. See issue #21 [here](https://github.com/NOAA-PMEL/uafnciso/issues/21).
