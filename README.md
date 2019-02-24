# NNAGD
Neural Network library for Analytical Gradient Descent interfaced with ceres-solver.
  
## Comparison
Fitting sin(x) with n=100 linear steps in x:

- **architecture[1,5,1]:**
  - **analytic**:		 time[1.218678 s]		iterations[1k] 	chi2/ndat[5.97889e-09]
  - **automatic**: 	 time[1.435668 s]		iterations[1k]		chi2/ndat[7.28241e-09]
  - **numeric**: 	  	 time[7.904501 s]		iterations[1k] 	chi2/ndat[7.28893e-09]  
    - **analytic ~ 15% numeric**
    - **automatic ~ 18% numeric**
    - **analytic ~ 84% automatic**  

- **architecture[1,10,1]:**
  - **analytic**:		 time[14.243720 s]		 iterations[10k] 	chi2/ndat[1.4889e-13]
  - **automatic**: 	 time[30.003974 s]		 iterations[10k]	chi2/ndat[1.4889e-13]
  - **numeric**: 	  	 time[177.566336 s]	 iterations[10k] 	chi2/ndat[1.77439e-13]  
    - **analytic ~ 8% numeric**
    - **automatic ~ 17% numeric**
    - **analytic ~ 47% automatic**  

- **architecture[1,20,1]:**
  - **analytic**:		 time[19.784494 s]		iterations[10k] 	chi2/ndat[3.78944e-14]
  - **automatic**: 	 time[80.598593 s]		iterations[10k]		chi2/ndat[3.78944e-14]
  - **numeric**: 	  	 time[475.223460 s]	iterations[10k] 	chi2/ndat[4.0141e-14]  
    - **analytic ~ 4% numeric**
    - **automatic ~ 17% numeric**
    - **analytic ~ 24.4% automatic**  

![](https://github.com/rabah-khalek/NNAGD/blob/master/output.png)
