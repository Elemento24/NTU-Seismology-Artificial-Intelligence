# General workflow of processing seismic data

## Step 5
- Convert the one-year-long mseed-format files into SAC-format files using the `mseed2sac.ipynb`.
- During the time, if you encounter errors related to response file, you can try `response_check.ipynb` to make recording duration compatible in response and mseed files. After checking response file, rerun `mseed2sac.ipynb`.

## Step 6
- Use Taup module in obspy to mark P-wave traveltime on the SAC-format waveform using the `parrival.ipynb`.

## Step 7
- Resample the SAC-format waveforms to a unified sampling rate - 20Hz (20 points per second) using the `filter_waveform.ipynb`.
- Bandpass filter the SAC-format waveforms (recommended bandpass: 0.02-2Hz)

## Step 8
- Calculate signal-to-noise ratio (SNR) for each SAC-format waveform, and based on which, to automatically select high-quality (high SNR) waveforms (recommended threshold: 3.0) using the `select_snr.ipynb`.

## Step 9
- Visualize the retained high-quality bandpass-filtered waveforms and the station and earthquakes distribution using the `quich_view.ipynb`.

