# Parameter-Optimisation-SVM


**Dataset Used:** [Dry bean Dataset](https://archive.ics.uci.edu/ml/datasets/Dry+Bean+Dataset)

| Number of Instances:  | 13000  |
|-----------------------|--------|
| Number of Attributes: | 17     |

---

**Parameter Grid Used**
---
|Hyperparameter         |Values                |
|-----------------------|----------------------|
| kernel                | 'linear', 'poly', 'rbf', 'sigmoid' |
| C                     | 0.001, 0.01, 0.1, 1, 10    |
| gamma                 |['scale', 'auto'] + list(np.logspace(-3, 3, 7))   |

---
 
 | Sample Number | Best Accuracy | Kernel | C  | gamma |
|----------|---------------|--------|-----|-------|
| 1        | 0.799       | rbf    | 1.000 | 0.001   |
| 2        | 0.765        |  poly    | 0.001 | scale   |
| 3        | 0.801        | rbf    | 10.000 | 0.01   |
| 4        | 0.801      | rbf    | 1.000 | auto   |
| 5        | 0.811       | rbf    | 1.000 | 0.1   |
| 6        | 0.799        | rbf    | 1.000 | 0.001  |
| 7        | 0.780        | rbf    | 1.000 | 0.1   |
| 8        | 0.799        | rbf    | 1.000 | 0.1   |
| 9        | 0.770        | rbf    | 1.000 | 0.1   |
| 10       | 0.784       | rbf    | 1.000 | 0.001 |

---

**Sample 5 gives the Best SVM accuracy with params: rbf,1.000,0.1 for Kernel,C and Gamma respectively**

---

Graph of Accuracy per 1000 iterations for Sample 5:

![alt text](https://github.com/UTK21/Parameter-optimisation-SVM/blob/main/screenshot.png)
