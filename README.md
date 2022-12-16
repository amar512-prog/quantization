# quantization
To quantize a self made model

###### For dynamic case: wts quantized, read act as fp32 and quant to compute
- We have dynamic quantized on assignment model to 8 bit integer.
* Accuracy of test case (w/o Q): 55.181818 %
* Accuracy of test case (w Q): 55.212121 %
* Time taken (w/o Q): 01:04 sec
* Time taken (w Q): 01:02 sec
+ Size (w/o Q): 3.15 MB and Size (w Q): 3.12 MB

###### For static case: wts quant, act quant, calibration post training
- We have static quantized on assignment model to 8 bit integer.
* Accuracy of test case (w/o Q): 55.181818 %
* Accuracy of test case (w Q): 55.030303 %, 
* Time taken: 00:38 sec, Time reduction = 59.375% 
+ Size(w/o Q): 809.9 KB = 0.79 MB, size reduction = 3.987 times


