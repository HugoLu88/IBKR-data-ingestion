# IBKR-data-ingestion
Dynamic data ingestion for the IBKR platform

This notebook requires the following inputs

1) Specify data to download from IBKR
2) Specify file directory

It will then do the following things

1) Check to see if there is anything in the file directory
2) If there is, append the latest data
3) If there is not, save the latest data

Note:

1) this will break if you try to overwrite data from say t0 to t1 with data from before t0. You can only append later data as this is supposed to be a rolling file where the dataset increases over time in a forward looking manner
