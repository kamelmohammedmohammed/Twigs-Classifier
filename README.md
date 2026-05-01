We propose the Twigs classifier — a new non-parametric method for classification. Unlike k-NN, which stores all training points, Twigs stores only 'boundary vectors' found by a novel algorithm called BVB (Boundary Vector Bisection). BVB pushes seeds toward class boundaries, independent of data dimensionality. A second version (BVBC) handles spiral problems. Classification then requires only a dot product. On 20 UCI datasets, Twigs outperforms k-NN, SVM, and even deep learning on several imbalanced and high-dimensional tasks. In 14 out of 20 cases, the misclassification rate was below 1%.

The purpose of the BVB and the BVBC algorithms is finding the Twigs (the BV and the 2 corresponding SVs)

Figure bellow shows how does the BVB algorithm uses the bisection method to obtain the boundary vectors (BVs) and the support vectors(SVs)

<img width="680" height="471" alt="image" src="https://github.com/user-attachments/assets/d0b643c5-5afb-4283-99e0-c4479f85d13b" />

Figure bellow presents the BVB algorithm behavior while finding twigs for three classes classification problem. It uses the bisection principle. 

<img width="1089" height="560" alt="image" src="https://github.com/user-attachments/assets/8f131042-4092-40c4-8dba-e34c5ec5ca4b" />

Twig definition: a twig is contructed by one boundary vector (BV) that is its a center and the two corresponding Support vectors (SVs)

<img width="933" height="459" alt="image" src="https://github.com/user-attachments/assets/416c6244-4c2a-4b21-b5cd-7d46b5b8694f" />

Classification rules:

<img width="666" height="197" alt="image" src="https://github.com/user-attachments/assets/4a9e7ca9-6bb2-4077-8107-d93368f601a5" />

When we perform a classification, the Twigs Classifier acts as an ensemble classification.
It uses both distance (nearest twig) and direction (its direction or orientation)

Twigs orientation optimization:

<img width="763" height="518" alt="image" src="https://github.com/user-attachments/assets/6c85a6a6-8771-4ca0-9b52-3960b4ec1d5e" />

The metric used for the otimization: (to find an orthogonal twigs to the boundary or to the separator)
<img width="426" height="113" alt="image" src="https://github.com/user-attachments/assets/19cd544e-5185-486a-9f7a-a1a2206acc36" />

Find the published paper:

Kamel Mebarkia, Aicha Reffad. Twigs classifiers based on the boundary vectors Machine (BVM): A novel approach for supervised learning.
Information Sciences, Volume 701, 2025, 121853, ISSN 0020-0255,
https://doi.org/10.1016/j.ins.2024.121853.
https://www.sciencedirect.com/science/article/abs/pii/S0020025524017675


