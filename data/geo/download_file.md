## Geographical Index Data

Geographical index data must be downloaded into the geo folder to operate the Fetch.R script. This index is provided with the program, but may be set to new definitions by regenerating the data. The index uses the 2010 geographical definitions and population counts and was generated with the [MCDC Geographic Correspondence Engine](http://mcdc.missouri.edu/applications/geocorr2014.html) under Rev. 9/10/2016.

The following settings must be selected.
* "Select the state(s) to process:" to select all with Shift+R.click
* "Select one or more source geographies:" to "ZIP/ZCTA" [under the heading "2010 Geographies:"]
* "Select one or more target geographies:" to "Core Based Statistical Area (CBSA)" [under the heading "2010 Geographies:"]
* "Weighting variable:" any [or "Population (2010 census)"]

Then select "Run request" with default settings.

This will produce a csv file with the proper variables. The name of the csv file must begin with "geo", and there should be only one such file in the geo folder at a time. A description csv file may be included with a name beginning with "desc". Note that the raw csv file will include a description for each variable in the second line that should be moved or deleted. Other years and weighting variables can be chosen with minor changes to the Fetch.R code, so long as the source and target geographies are set to ZIP/ZCTA and CBSA, respectively.
