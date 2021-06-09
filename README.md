# PINNeikonal
Eikonal solution using physics-informed neural networks

The eikonal equation is utilized across a wide spectrum of science and engineering disciplines. In seismology, it regulates seismic wave traveltimes needed for applications like source localization, imaging, and inversion. Several numerical algorithms have been developed over the years to solve the eikonal equation. However, these methods require considerable modifications to incorporate additional physics, such as anisotropy, and may even breakdown for certain complex forms of the eikonal equation, requiring approximation methods. Moreover, they suffer from computational bottleneck when repeated computations are needed for perturbations in the velocity model and/or the source location, particularly in large 3D models. Here, we propose an algorithm to solve the eikonal equation based on the emerging paradigm of physics-informed neural networks (PINNs). By minimizing a loss function formed by imposing the eikonal equation, we train a neural network to output traveltimes that are consistent with the underlying partial differential equation. We observe sufficiently high traveltime accuracy for most applications of interest. We also demonstrate how the proposed algorithm harnesses machine learning techniques like transfer learning and surrogate modeling to speed up traveltime computations for updated velocity models and source locations. Furthermore, we use a locally adaptive activation function and adaptive weighting of the terms in the loss function to improve convergence rate and solution accuracy. We also show the flexibility of the method in incorporating medium anisotropy and free-surface topography compared to conventional methods that require significant algorithmic development. These properties of the proposed PINN eikonal solver are highly desirable in obtaining a flexible and efficient forward modeling engine for seismological applications.

## Libraries
The scripts work with Tensorflow v2.2.0 and SciAnn v0.5.4.0


## Citation
If you find our work useful in your research, please cite:
```
@article{bin2021pinneik,
  title={PINNeik: Eikonal solution using physics-informed neural networks},
  author={bin Waheed, Umair and Haghighat, Ehsan and Alkhalifah, Tariq and Song, Chao and Hao, Qi},
  journal={Computers \& Geosciences},
  pages={104833},
  year={2021},
  publisher={Elsevier}
}
```

## Contact
If you have any questions, please feel free to email the author.
