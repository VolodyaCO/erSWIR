# erSWIR
Replication of SWIR model in ER networks

Install graph-tool in linux with Anaconda using this tutorial:
https://medium.com/@ronie/installing-graph-tool-for-python-3-on-anaconda-3f76d9004979


## Data:
### 1
* nodes: 1M -> N
* samples: 3k -> n
* name: `"results/{0}_{1}_rho_sub_critical.p".format(n,N)`
~~~~
max_new = 0.115+0.003
min_new = 0.115-0.003
kappa_range = (kappa_range-kappa_range.min()) * (max_new - min_new) / 2 + min_new
~~~~
### 2
* nodes: 1M -> N
* samples: 3k -> n
* name: `"results/{0}_{1}_rho_critical.p".format(n,N)`
~~~~
max_new = 0.108021+0.003
min_new = 0.108021-0.003
kappa_range = (kappa_range-kappa_range.min()) * (max_new - min_new) / 2 + min_new
~~~~
### 3
* nodes: 50k -> N
* samples: 20k -> n
* name: `"results/{0}_{1}_rho_critical.p".format(n,N)`
~~~~
max_new = 0.108021+0.003
min_new = 0.108021-0.003
kappa_range = (kappa_range-kappa_range.min()) * (max_new - min_new) / 2 + min_new
~~~~
### 4 
* samples: 6k -> n
* name: `"results/{0}_fig7_rho_sub_critical.p".format(n)`
`N_range = [int(n) for n in np.geomspace(1e5, 3e6, 10)]`
### 5
* samples: 65k -> n
* name: `"results/{0}_fig7_rho_sub_critical.p".format(n)`
`N_range = [ 100000,  145923,  212936, 310723]`
### 6
* samples: 32k -> n
* name: `"results/{0}_fig10_rho_critical.p".format(n)`
`N_range = [ 100000,  145923,  212936, 310723]`
### 7
* samples: 1000 -> n (for each N)
* nodes: 100000,  145923,  212936, 310723 -> N
* name: `'./results/{0}_{0}_fig10_rho_critical.p'.format(num_ensamble, N)`
