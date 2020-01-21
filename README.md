# SVM-implimentation-on-IRIS-dataset

SVM can be implemented using sklearn by 2 methods:sklearn.svm.LinearSVC (mostly fpr linear) and  sklearn.svm.SVC.

sklearn.svm.LinearSVC is similar to sklearn.svm.SVC except it is implemented in terms of liblinear rather than libsvm, so it has more flexibility in the choice of penalties and loss functions and should scale better to large numbers of samples.

Also A Support Vector Machine is essentially a Quadratic Programming (QP) problem. This optimization problem has two forms (a primal and a dual). The Quadratic program solver used in libSVM is targeted to work for both linear and non-linear kernel. The training time complexity is somewhere around O(n2) to O(n3). The solver in libLinear is targeted to primarily work with linear kernel and on top of that it offers several variations (L1/L2 regularization, L1/L2 loss etc.). The training time complexity is somewhere around O(n).

(source:https://www.quora.com/Whats-the-difference-between-LibSVM-and-LibLinear)

sklearn.svm.SVC (https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC):

There are different kernels used for approximation:‘linear’, ‘poly’, ‘rbf’, ‘sigmoid’.
