## Auto Sklearn results:
| | knn 1h | sgd 1h | svr 1h | linear svr 1h | extra trees 1h | decision tree 1h | random forest 1h | neural network 1h | adaboost 1h | random search 1h
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **95 features** | 2.46 | 3.30 | 2.55 | 1.59 | 1.77 | 2.51 | 2.15 | 0.63 | 1.77 |  1.01
| **35 features** | 1.94 | 2.42 | 3.47 | 1.59 | 1.85 | 2.14 | 2.03 | 0.31 | 1.88 |  0.43
| **6 features** | 2.03 | 2.88 | 4.84 | 1.91 | 1.81 | 2.07 | 2.07 | 0.87 | 1.81 |  2.73
| **16 features** | 3.14 | 4.22 | 4.32 | 2.63 | 1.80 | 2.15 | 1.96 | 1.76 | 1.93 |  1.26

## Permutation importance: original features (16 features):
|  | 1st | 2ed | 3rd | 4th | 5th | 6th | 7th | 8th | 9th | 10th
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **knn** | SPEED | ENGINE_LOAD  | ENGINE_RPM  | FUEL_LEVEL  | ENGINE_RUNTIME | INTAKE_MANIFOLD_PRESSURE | MAF | FUEL_RATE | AMBIENT_AIR_TEMP | AIR_INTAKE_TEMP |
| **sgd** | SPEED     | MAF       | FUEL_RATE  | ENGINE_LOAD  | ENGINE_RPM  | TIMING_ADVANCE  | FUEL_LEVEL  | ENGINE_RUNTIME  | THROTTLE_POS  | AIR_INTAKE_TEMP |
| **svr** | SPEED     | FUEL_RATE  | MAF       | TIMING_ADVANCE  | FUEL_LEVEL  | AIR_INTAKE_TEMP | ENGINE_RPM  | INTAKE_MANIFOLD_PRESSURE  | BAROMETRIC_PRESSURE(KPA) | - |
| **linear svr** | SPEED     | MAF       | FUEL_RATE  | ENGINE_LOAD  | ENGINE_RPM  | TIMING_ADVANCE  | FUEL_LEVEL  | THROTTLE_POS  | ENGINE_RUNTIME  | - | 
| **extra trees** | SPEED     | FUEL_RATE  |MAF       | ENGINE_RPM  | ENGINE_LOAD  | THROTTLE_POS  | TIMING_ADVANCE  | FUEL_LEVEL  | ENGINE_RUNTIME  | - | 
| **decision tree** | SPEED     | THROTTLE_POS  | MAF       | FUEL_RATE  | ENGINE_LOAD  | - | - | - | - |  - |
| **random forest** | SPEED     | FUEL_RATE  | MAF       | ENGINE_RPM  | THROTTLE_POS  | ENGINE_LOAD  | - | - | - | - |
| **neural network** | SPEED     | FUEL_LEVEL | ENGINE_LOAD  | MAF      | FUEL_RATE  | THROTTLE_POS  | INTAKE_MANIFOLD_PRESSURE  | - | - | - | 
| **adaboost** | SPEED     | FUEL_RATE  | MAF       | THROTTLE_POS  | ENGINE_LOAD  | - | - | - | - | - |16 