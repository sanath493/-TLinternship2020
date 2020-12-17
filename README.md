# TLinternship2020
The code is in the form of a ipython notebook
It needs to be run along with the ward.paths.gz files in within the same folder.These files can be found in the repository.
The code is takes very long time to give the outputs due to the large amouont of data.
The output will be a list of dictionaries containing the covid related htmls under their particular months as keys.

Approach:

1)First we read all the warc.gz files from the path files of each month 


2)We then check if the urls inside the warc files are related to covid by using check_if_covid function which inturn reads the data
from the html files,beautifies it.


3)This data is then split using nltk tokenizer t get the words and then we check if they match the key words(corona in this case).


4)If they match then the url is aaved and returned.


5)This process repeats until we find 1000(can be given as sys argument) covid related urls.

Results & Analysis:
Tried checking for urls for almost 3hrs on a 16GB RAM GPU based machine.
Most of the links were Chinese or Russian spam links. do I couldn't find much information there

Checked the functions for a custom list of covid urls and the code detects them well.

Edit:I will be uploading some screenshots soon
