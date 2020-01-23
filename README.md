# ecg-extract

Extract and analyze ECG signal from apple ECG report.


## ecg-extract.ipynb

Newer Apple watches include 'ECG' functionality, however there is currently no public API to access ECG data.

This notebook attempts to recreate the ECG data using the exported PDF of the ECG report.

1. PDF was converted to png using preview. (File -> Export -> Format=PNG Resolution=150 pixel/inch)
2. ECG sections of the report are extracted and stitched together.
3. Waveform is pulled out using argmin
4. Analysis of ECG using heartpy

