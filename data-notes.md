# MassDOT Impact Person Level Crash Data

## Overview 

 - Crash incident data for 5.7 million individuals involved in crashes in MA, from 2002 to 2019
 - Full data set uncompressed size ~20 GB
 - 2020-2022 are available but MassDot Impact says they are not authoritative yet
 - Person-level: there are usually multiple records per crash that must be deduplicated. State crash-level data might offer more information about the crash itself, unknown.
 - Fields like the below contain nested key-value pairs:  
   MOST\_HRMFUL\_EVT\_CL : V1:(Collision with cyclist (bicycle, tricycle, unicycle, pedal car))

### 2010

2010 is missing the person-level fields. A download was done manually from the MassDOT Impact Query & Visualization tool using the query `SELECT * FROM tableName WHERE crash_date BETWEEN '1/1/2010' AND '12/31/2010' AND pers_type = 'Non-motorist'`.

## Links

 - [Home page](https://apps.impact.dot.state.ma.us/cdp/home)
 - [E.S.R.I. Open Data Portal](https://massdot-impact-crashes-vhb.opendata.arcgis.com/search?collection=Dataset&sort=-modified)
 - [2021 Codebook](https://gis.impact.dot.state.ma.us/arcgis/rest/services/MassDOT/MASSDOT_ODP_OPEN_2021/FeatureServer/layers)

## Downloading

On Massdot's E.S.R.I. data portal:

 1. Search "Person level"
 2. Click a set, viewer will open
 3. Click "view full details"
 4. Click Download
