General workflow of processing seismic data.
################################

***step5***  -- 5.mseed2sac.ipynb
Convert the one-year-long mseed-format files into SAC-format files. During the time, if you encounter errors related to response file, you can try response_check.ipynb to make recording duration compatible in response and mseed files. After checking response file, rerun mseed2sac.

***step6***  -- 6.parrival.ipynb
Use Taup module in obspy to mark P-wave traveltime on the SAC-format waveform.

***step7***  -- 7.filter_waveform.ipynb
Resample the SAC-format waveforms to a unified sampling rate - 20Hz (20 points per second)
Bandpass filter the SAC-format waveforms (recommended bandpass: 0.02-2Hz)

***step8***  -- 8.select_snr.ipynb
Calculate signal-to-noise ratio (SNR) for each SAC-format waveform, and based on which, to automatically select high-quality (high SNR) waveforms (recommended threshold: 3.0)


***step9***  -- 9.quich_view.ipynb
Visualize the retained high-quality bandpass-filtered waveforms and the station and earthquakes distribution.

