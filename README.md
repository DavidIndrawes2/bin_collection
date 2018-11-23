# bin_collection

To find out the bin collection events for certain date,run the `bin_collection.py` script.

The script takes two arguments
1. URL: the url for the .ical file with the collection data
2. Date: the date you want to to check, the date has to be in `YYYYMMDD` format, for example: `20181226`

for example run the following command to check what events do you have on the 12th June 2018
Some basic Git commands are:
```
python bin_collection.py https://s3-eu-west-1.amazonaws.com/fs-downloads/GM/binfeed.ical 20180612
```
you should get the following output
```
Blue Bin Collection
Green Bin Collection
```