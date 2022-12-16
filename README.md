# quantization
To quantize a self made model

###### For dynamic case: weights quantized, activation as fp32 from test input and quantized to compute
- We have dynamic quantized on assignment model to 8 bit integer.
* Accuracy of test case (w/o Q): 55.181818 %
* Accuracy of test case (w Q): 55.212121 %
* Time taken (w/o Q): 01:04 sec
* Time taken (w Q): 01:02 sec
+ Size (w/o Q): 3.15 MB and Size (w Q): 3.12 MB

###### For static case: weights quantized, activation from training input as calibration and quantized as precomputation of testing
- We have static quantized on assignment model to 8 bit integer.
* Accuracy of test case (w/o Q): 55.181818 %
* Accuracy of test case (w Q): 55.030303 %, 
* Time taken: 00:38 sec, Time reduction = 59.375% 
+ Size(w/o Q): 809.9 KB = 0.79 MB, size reduction = 3.987 times


