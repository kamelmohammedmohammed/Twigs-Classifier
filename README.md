We propose the Twigs classifier — a new non-parametric method for classification. Unlike k-NN, which stores all training points, Twigs stores only 'boundary vectors' found by a novel algorithm called BVB (Boundary Vector Bisection). BVB pushes seeds toward class boundaries, independent of data dimensionality. A second version (BVBC) handles spiral problems. Classification then requires only a dot product. On 20 UCI datasets, Twigs outperforms k-NN, SVM, and even deep learning on several imbalanced and high-dimensional tasks. In 14 out of 20 cases, the misclassification rate was below 1%.

The purpose of the BVB and the BVBC algorithms is finding the Twigs (the BV and the 2 corresponding SVs)
<img width="1342" height="756" alt="image" src="https://github.com/user-attachments/assets/58160cac-8a1c-4e40-be7a-e0937acc60cc" />

Twigs definition:
<img width="1166" height="574" alt="image" src="https://github.com/user-attachments/assets/9e734493-8cdc-4ee7-92f7-6afba1acc88d" />

Classification rules:
<img width="666" height="197" alt="image" src="https://github.com/user-attachments/assets/b8d02a79-6700-4dc4-aeaf-18ba398a11df" />
Twigs pruning:
<img width="1040" height="706" alt="image" src="https://github.com/user-attachments/assets/35bf10d4-3d88-4ff5-bb15-16cf469ddb4f" />

the metric used for the pruning:
<img width="426" height="113" alt="image" src="https://github.com/user-attachments/assets/19cd544e-5185-486a-9f7a-a1a2206acc36" />




