# data-512-a1
 Data512 Assignment A1 - Richard Todd

# Project goal and purpose
The goal of this assignment is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2019. The purpose of the assignment is to explore and to demonstrate best practices for open scientific research in designing and implementing a simple project, and in doing so make the project fully reproducible by others.

# License
Source data is made available by the Wikimedia Foundation under a CC-BY-SA 30 license. The Wikimedia Foundation REST API terms of use are available at: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

This code is made available under an MIT license (see license.txt).

# API documentation
API documentation is available at https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews (Pageview) and https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts (Pagecount)

This code is made available for re-use under a [CC0 license](https://creativecommons.org/share-your-work/public-domain/cc0/). 

# Exported data 
The final datafile - en-wikipedia_traffic_200712-201809.csv - contains pageview statistics for English Wikipedia from 2008 to August 2019. It contains the followign fields: 'year' (YYYY),  'month' (MM),  'pagecount_all_views' (no. of views, numeric), 'pagecount_desktop_views' (no. of views, numeric), 'pagecount_mobile_views' (no. of views, numeric), 'pageview_all_views' (no. of views, numeric),  'pageview_desktop_views' (no. of views, numeric), and 'pageview_mobile_views' (no. of views, numeric)

# Other files
Included in this repository are JSON files of data retrieved from the APIS (September 2019) and a visualization produced by the script.


# Known issues and special considerations
Data from the Pageview API - available from 2015 onwards - excludes non-human (i.e.spider & crawler) traffic), while data from the legacy Pagecount API does not enable this filtering. The Pageview API also distinguishes between mobile app and mobile site traffic, which is combined in this analysis for the purpose of comparability with the legacy Pagecount API data.