# MPG.PuRe to CSV
The 'MPG.PuRe to CSV' script enables the creation of simple CSV lists out of the publication repository of the Max Planck Society (https://pure.mpg.de/).

To create your individual query on the MPG.PuRe interface, first use the Advanced Search there and enter the desired search parameters.
On the search result page, select the "Insert query in REST interface" function.
This takes you to a form including the ElasticSearch query you just created. You may ignore the settings regarding export formats at this point: the required Json format will automatically be selected by the script.
If desired, you can also set individual sorting criteria and sorting order here.
You can now download the CURL command for your search using the corresponding button.

You will need to fill in the entire '{"query" : ...' part of the command - as shown in the example query of the script.

No login information is required to perform the export via the script.

The fields extracted from MPG.PuRe by default are:
- Item-ID (including version number)
- Creators
- Title
- Genre
- Publication Status
- Date (of the highest ranking category)
- Open Access Status
- Local Tag

You can access and execute the skript directly via MyBinder and adapt the parameters according to your requirements. 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LeimLarissa/PuRe-to-CSV/HEAD)
