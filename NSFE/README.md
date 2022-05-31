# General workflow of preparing seismic data

## Step 0
- Prepare the earthquake catalog in 1 year each time. Goal is to cover the earthquake data from 2000 to 2022.
- Extract the earthquake catalog, i.e., the location of earthquakes including the longitude, latitude, depth and magnitude from USGS catalog.

## Step 1
- Modify the study region, which is defined as a rectangular. Its four end-points mean minlat -- minimum latitude, maxlat -- maximum latitude, minlon -- minimum longitude, maxlon -- maximum longitude; Note the time duration should be consistent with you catalog data, e.g., if catalog 2021.01.01 - 2022.01.01, then stations 2021.01.01 - 2022.01.01
- Download the list of seismic stations, i.e., the location of stations including the longitude, latitude and elevation above sea-level.

## Step 2
- Modify the study region, which is defined as a rectangular. Its four end-points mean minlat -- minimum latitude, maxlat -- maximum latitude, minlon -- minimum longitude, maxlon -- maximum longitude
- Make the plot to show the distribution of earthquakes and seismic stations in our study region.

## Step 3 
- Download waveforms from event origin time to one hour after.
- Download the seismic waveforms from available seismic networks in our study region. The downloaded data are in format of miniseed, and we will transform it into the format of SAC, which is more convenient for us to deal with.

## Step 4
- Try to visualize more waveforms and get sense of waveform quality and its dependece on earthquake magnitude
- Quickly view seismic waveforms for several events.

