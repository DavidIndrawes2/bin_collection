# bin_collection

To find out the next available bin collection events for a given date,run the `bin_collection.py` script.
The scripts return all the events in the next collection day, if the day given is a collection day it will return the events in the given date

The script takes two arguments
1. URL: the url for the .ical file with the collection data
2. Date: the date you want to to check, the date has to be in `YYYYMMDD` format, for example: `20181226`


for example run the following command to check what events do you have on the 12th June 2018
```
python bin_collection.py https://s3-eu-west-1.amazonaws.com/fs-downloads/GM/binfeed.ical 20180612
```
you should get the following output
```
The next collection will be on 20180612
What bins will be collected:
Blue Bin Collection
Green Bin Collection
```

or run the following to see when is the next collection day after the 11th June 2018
```
python bin_collection.py https://s3-eu-west-1.amazonaws.com/fs-downloads/GM/binfeed.ical 20180611
```
you should get the following output
```
The next collection will be on 20180612
What bins will be collected:
Blue Bin Collection
Green Bin Collection
```