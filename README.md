# Supplementary material: Triplet attack
Currently Loaded Modules:
  1) cuda/11.0   2) cudnn/11.0-8.0.3.33

 

now processing task id::  1
2022-01-12 17:18:05.893127: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudart.so.11.0
2022-01-12 17:19:09.757865: I tensorflow/compiler/jit/xla_cpu_device.cc:41] Not creating XLA devices, tf_xla_enable_xla_devices not set
2022-01-12 17:19:09.772793: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcuda.so.1
2022-01-12 17:19:09.849566: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1720] Found device 0 with properties: 
pciBusID: 0000:8a:00.0 name: NVIDIA GeForce GTX 1080 Ti computeCapability: 6.1
coreClock: 1.582GHz coreCount: 28 deviceMemorySize: 10.92GiB deviceMemoryBandwidth: 451.17GiB/s
2022-01-12 17:19:09.849642: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudart.so.11.0
2022-01-12 17:19:09.856537: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublas.so.11
2022-01-12 17:19:09.856750: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublasLt.so.11
2022-01-12 17:19:09.861718: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcufft.so.10
2022-01-12 17:19:09.864381: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcurand.so.10
2022-01-12 17:19:09.871089: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcusolver.so.10
2022-01-12 17:19:09.873951: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcusparse.so.11
2022-01-12 17:19:09.884177: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudnn.so.8
2022-01-12 17:19:09.896564: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1862] Adding visible gpu devices: 0
2022-01-12 17:19:09.897406: I tensorflow/compiler/jit/xla_gpu_device.cc:99] Not creating XLA devices, tf_xla_enable_xla_devices not set
2022-01-12 17:19:09.898860: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1720] Found device 0 with properties: 
pciBusID: 0000:8a:00.0 name: NVIDIA GeForce GTX 1080 Ti computeCapability: 6.1
coreClock: 1.582GHz coreCount: 28 deviceMemorySize: 10.92GiB deviceMemoryBandwidth: 451.17GiB/s
2022-01-12 17:19:09.898920: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudart.so.11.0
2022-01-12 17:19:09.899006: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublas.so.11
2022-01-12 17:19:09.899065: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublasLt.so.11
2022-01-12 17:19:09.899115: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcufft.so.10
2022-01-12 17:19:09.899155: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcurand.so.10
2022-01-12 17:19:09.899191: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcusolver.so.10
2022-01-12 17:19:09.899226: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcusparse.so.11
2022-01-12 17:19:09.899263: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudnn.so.8
2022-01-12 17:19:09.901421: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1862] Adding visible gpu devices: 0
2022-01-12 17:19:09.917182: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudart.so.11.0
2022-01-12 17:19:13.741359: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1261] Device interconnect StreamExecutor with strength 1 edge matrix:
2022-01-12 17:19:13.741433: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1267]      0 
2022-01-12 17:19:13.741448: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1280] 0:   N 
2022-01-12 17:19:13.745468: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1406] Created TensorFlow device (/job:localhost/replica:0/task:0/device:GPU:0 with 10269 MB memory) -> physical GPU (device: 0, name: NVIDIA GeForce GTX 1080 Ti, pci bus id: 0000:8a:00.0, compute capability: 6.1)
2022-01-12 17:19:15.168370: I tensorflow/compiler/mlir/mlir_graph_optimization_pass.cc:116] None of the MLIR optimization passes are enabled (registered 2)
2022-01-12 17:19:15.169271: I tensorflow/core/platform/profile_utils/cpu_utils.cc:112] CPU Frequency: 2100085000 Hz
2022-01-12 17:19:17.775159: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublas.so.11
2022-01-12 17:19:18.151492: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcublasLt.so.11
2022-01-12 17:19:18.334023: I tensorflow/stream_executor/platform/default/dso_loader.cc:49] Successfully opened dynamic library libcudnn.so.8
Profiling traces number: 50000
Attack traces number: 10000
Add desync noise...
Add desync noise...
=============ASCAD_HW_Triplet_ep1_BS512_ES32_desync0.0_alpha0.1_margin0.4_1=============
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv1d (Conv1D)              (None, 4000, 64)          1024      
_________________________________________________________________
average_pooling1d (AveragePo (None, 266, 64)           0         
_________________________________________________________________
conv1d_1 (Conv1D)            (None, 266, 128)          24704     
_________________________________________________________________
average_pooling1d_1 (Average (None, 133, 128)          0         
_________________________________________________________________
Flatten (Flatten)            (None, 17024)             0         
_________________________________________________________________
dense (Dense)                (None, 32)                544800    
=================================================================
Total params: 570,528
Trainable params: 570,528
Non-trainable params: 0
_________________________________________________________________
98/98 - 21s - loss: 0.1422 - val_loss: 0.0342
======Tamplate attack======
0/10000
2000/10000
4000/10000
6000/10000
8000/10000
GE:  0.0
GE smaller than 1: 200
GE smaller than 5: 125
Print and save GE TA
=============ASCAD_ID_Triplet_ep1_BS512_ES32_desync0.0_alpha0.1_margin0.4_1=============
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv1d_2 (Conv1D)            (None, 4000, 64)          1024      
_________________________________________________________________
average_pooling1d_2 (Average (None, 266, 64)           0         
_________________________________________________________________
conv1d_3 (Conv1D)            (None, 266, 128)          24704     
_________________________________________________________________
average_pooling1d_3 (Average (None, 133, 128)          0         
_________________________________________________________________
Flatten (Flatten)            (None, 17024)             0         
_________________________________________________________________
dense_1 (Dense)              (None, 32)                544800    
=================================================================
Total params: 570,528
Trainable params: 570,528
Non-trainable params: 0
_________________________________________________________________
98/98 - 15s - loss: 0.1630 - val_loss: 0.0509
======Tamplate attack======
0/10000
2000/10000
4000/10000
6000/10000
8000/10000
GE:  0.0
GE smaller than 1: 84
GE smaller than 5: 40
Print and save GE TA
Profiling traces number: 50000
Attack traces number: 10000
Add desync noise...
Add desync noise...
=============ASCAD_rand_HW_Triplet_ep1_BS512_ES32_desync0.0_alpha0.1_margin0.4_1=============
Model: "sequential_2"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv1d_4 (Conv1D)            (None, 4000, 64)          1024      
_________________________________________________________________
average_pooling1d_4 (Average (None, 266, 64)           0         
_________________________________________________________________
conv1d_5 (Conv1D)            (None, 266, 128)          24704     
_________________________________________________________________
average_pooling1d_5 (Average (None, 133, 128)          0         
_________________________________________________________________
Flatten (Flatten)            (None, 17024)             0         
_________________________________________________________________
dense_2 (Dense)              (None, 32)                544800    
=================================================================
Total params: 570,528
Trainable params: 570,528
Non-trainable params: 0
_________________________________________________________________
98/98 - 15s - loss: 0.1456 - val_loss: 0.0976
======Tamplate attack======
0/10000
2000/10000
4000/10000
6000/10000
8000/10000
GE:  0.0
GE smaller than 1: 180
GE smaller than 5: 98
Print and save GE TA
=============ASCAD_rand_ID_Triplet_ep1_BS512_ES32_desync0.0_alpha0.1_margin0.4_1=============
Model: "sequential_3"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv1d_6 (Conv1D)            (None, 4000, 64)          1024      
_________________________________________________________________
average_pooling1d_6 (Average (None, 266, 64)           0         
_________________________________________________________________
conv1d_7 (Conv1D)            (None, 266, 128)          24704     
_________________________________________________________________
average_pooling1d_7 (Average (None, 133, 128)          0         
_________________________________________________________________
Flatten (Flatten)            (None, 17024)             0         
_________________________________________________________________
dense_3 (Dense)              (None, 32)                544800    
=================================================================
Total params: 570,528
Trainable params: 570,528
Non-trainable params: 0
_________________________________________________________________
98/98 - 15s - loss: 0.1938 - val_loss: 0.0913
======Tamplate attack======
0/10000
2000/10000
4000/10000
6000/10000
8000/10000
GE:  0.0
GE smaller than 1: 131
GE smaller than 5: 52
Print and save GE TA
Add desync noise...
Add desync noise...
=============AESHD_HW_Triplet_ep1_BS512_ES32_desync0.0_alpha0.9_margin0.4_1=============
Model: "sequential_4"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv1d_8 (Conv1D)            (None, 1250, 64)          1024      
_________________________________________________________________
average_pooling1d_8 (Average (None, 83, 64)            0         
_________________________________________________________________
conv1d_9 (Conv1D)            (None, 83, 128)           24704     
_________________________________________________________________
average_pooling1d_9 (Average (None, 41, 128)           0         
_________________________________________________________________
Flatten (Flatten)            (None, 5248)              0         
_________________________________________________________________
dense_4 (Dense)              (None, 32)                167968    
=================================================================
Total params: 193,696
Trainable params: 193,696
Non-trainable params: 0
_________________________________________________________________
88/88 - 10s - loss: 0.2414 - val_loss: 0.1750
======Tamplate attack======
0/5000
2000/5000
4000/5000
GE:  0.0
GE smaller than 1: 2134
GE smaller than 5: 1574
Print and save GE TA
