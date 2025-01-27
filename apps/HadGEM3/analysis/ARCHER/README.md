# Results for the HadGEM3-GC31_benchmark on ARCHER

* The timings are averaged over five runs ± standard deviation.
* See ```coupled_run.job``` to understand how the total number of nodes is calculated depending on the UM and the nemo grid sizes.
  * We use two OpenMP threads per process for the UM-model.
  * We use eight XIOS processors.
 * We use the ```UM Run job``` start and end time from ```pe_output/atmos.fort6.pe0``` here, which is slighlty shorter than the overall run time for the batch script (can vary from less than 2% to - rarely - 17%).

UM_ATM_NPROCX | UM_ATM_NPROCY| NEMO_IPROC (jpni) | NEMO_JPROC (jpnj) | total number of nodes | UM time (sec)| total run time(s)
---- | -------|--------|---------|--------|----------|---------------
 48 | 37 | 24 |36 | 189 | 1569.80±88.53 | 1667.20±82.46
 36 | 37 | 24 |36 | 152 | 1801.60±106.90 | 1877.00±93.74
 60 | 47 | 24 |36 | 276 | 1484.20±71.26 | 1651.80±71.60
 60 | 47 | 33 |42 | 298 | 1579.00±119.66 | 1761.40±155.40
 48 | 37 | 33 |42 | 211 | 1680.00±148.16| 1797.00±141.30
 48 | 37 | 12 |18 | 168 | 1793.80±24.55 | 1864.00±16.17
 
 
UM_ATM_NPROCX | UM_ATM_NPROCY| NEMO_IPROC (jpni) | NEMO_JPROC (jpnj) | total number of nodes | UM time (sec)| total run time(s)
---- | -------|--------|---------|--------|----------|---------------
 48 | 37 | 24 |36 | 189 |  1491,1484,1620,1561,1639| 1667.20±82.46
 36 | 37 | 24 |36 | 152 |  1883,1680,1934,1720,1791| 1877.00±93.74
 60 | 47 | 24 |36 | 276 |  1484,1529,1528,1519,1361| 1651.80±71.60
 60 | 47 | 33 |42 | 298 |  1770,1603,1557,1459,1506| 1761.40±155.40
 48 | 37 | 33 |42 | 211 |  1924,1578,1610,1572,1716| 1797.00±141.30
 48 | 37 | 12 |18 | 168 |  1777,1770,1830,1785,1843| 1864.00±16.17
