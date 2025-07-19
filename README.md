# Multi-view_attention_fusion_for_AMC
A Multi-View Attention Fusion model for Automatic Modulation Classification. 
Fuses three different perspective of the dataset i.e., RML2016.10a_dict.pkl together.
The three branches are Temporal, Spectral and Statistical.
Temporal: Uses 1D CNN to extract time domain insights.
Spectral: Uses 2D CNN to capture time-frequency domain features from signals processed using Short-Time Fourier Transform. Also, uses Squeeze and Excitation channel attention.
Statistical: Uses a dense layer to process mean, range and standard deviation.
Dense layers are then used to fuse the three branches together.
A bidirectional GRU is used for comaparison.
