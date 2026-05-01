We propose the Twigs classifier — a new non-parametric method for classification. Unlike k-NN, which stores all training points, Twigs stores only 'boundary vectors' found by a novel algorithm called BVB (Boundary Vector Bisection). BVB pushes seeds toward class boundaries, independent of data dimensionality. A second version (BVBC) handles spiral problems. Classification then requires only a dot product. On 20 UCI datasets, Twigs outperforms k-NN, SVM, and even deep learning on several imbalanced and high-dimensional tasks. In 14 out of 20 cases, the misclassification rate was below 1%.

The purpose of the BVB and the BVBC algorithms is finding the Twigs (the BV and the 2 corresponding SVs)

Figure bellow shows how does the BVB algorithm uses the bisection method to obtain the boundary vectors (BVs) and the support vectors(SVs)

<img width="1174" height="813" alt="image" src="https://github.com/user-attachments/assets/a8f8637c-6bd6-42e9-ab3f-943914c70b39" />

Figure bellow presents the BVB algorithm behavior while finding twigs for three classes classification problem. It uses the bisection principle. 
<img width="1342" height="756" alt="image" src="https://github.com/user-attachments/assets/58160cac-8a1c-4e40-be7a-e0937acc60cc" />

Twig definition: a twig is contructed by one boundary vector (BV) that is its a center and the two corresponding Support vectors (SVs)

<img width="1166" height="574" alt="image" src="https://github.com/user-attachments/assets/9e734493-8cdc-4ee7-92f7-6afba1acc88d" />

Classification rules:
<img width="666" height="197" alt="image" src="https://github.com/user-attachments/assets/b8d02a79-6700-4dc4-aeaf-18ba398a11df" />

When we perform a classification, the Twigs Classifier acts as an ensemble classification.
It uses both distance (nearest twig) and direction (its direction or orientation)

Twigs orientation optimization:
<img width="1040" height="706" alt="image" src="https://github.com/user-attachments/assets/35bf10d4-3d88-4ff5-bb15-16cf469ddb4f" />

the metric used for the otimization: (to find an orthogonal twigs to the boundary or to the separator)
<img width="426" height="113" alt="image" src="https://github.com/user-attachments/assets/19cd544e-5185-486a-9f7a-a1a2206acc36" />

Find the published paper:

Kamel Mebarkia, Aicha Reffad. Twigs classifiers based on the boundary vectors Machine (BVM): A novel approach for supervised learning.
Information Sciences, Volume 701, 2025, 121853, ISSN 0020-0255,
https://doi.org/10.1016/j.ins.2024.121853.
https://www.sciencedirect.com/science/article/abs/pii/S0020025524017675


