# Physics-Informed ML Surrogate for Chemical Reactors

An end-to-end data-driven surrogate model predicting product yield in a non-isothermal plug-flow reactor.

### Project Architecture
* **Kinetics:** Modeled the consecutive reaction network A -> B -> C.
* **Feature Engineering:** Derived physical features including linearized Arrhenius temperature dependencies and logarithmic residence time.
* **Mechanistic Surrogate:** Fitted rate constants via Differential Evolution global optimization.
* **Hybrid Ensemble:** Combined the analytical kinetic predictions with an optimal blend of SVR (RBF Kernel) and Gradient Boosting.

### Performance Benchmarks
* **Naive Baseline CV RMSE:** 38.25
* **Vanilla GBM CV RMSE:** 19.53
* **Final Hybrid Ensemble CV RMSE:** 16.72
