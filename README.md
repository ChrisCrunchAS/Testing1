# Testing1
First try at the Alphasense Data set taken over two summer months

sensormatrix.h5 is the artificial matrix constructed by slicing a 60 minute time window across the WE for the N02 sensor. Similarly, referencematrix.h5 is the "ref_NO2 / ppb " column, changed into the same size 60 x 80000 matrix.

This is the first run through of the CNN. We try to train each 60 x 1 vector (80,000 of them) in our network.

After converting these matrices into LMDB format, the real test begins. There are many errors with my net in caffe. 
My understanding of how the network is interpretting the data is still pretty hazy. I may try using the raw hdf5 layer for data input now.
