# Structured Neural-PI Control for Networked Systems: Stability and Steady-State Optimality Guarantee
This repository contains source code necessary to reproduce the results presented in the following paper:
Structured Neural-PI Control for Networked Systems: Stability and Steady-State Optimality Guarantee 




# Motivation
We study the control of safety-critical networked systems with the goal of optimizing both transient and steady-state performances. Linear Proportional-Integral (PI)  controllers are almost always used in practice, but the linear parameterization of the controller limits its degrees of freedom for optimizing performances. Learning-based approaches are becoming popular in designing nonlinear controllers, but the lack of stability guarantee makes the learned controllers difficult to apply for practical applications. 

This paper bridges the gap between neural network-based controller design and stability guarantees. Using a property called equilibrium-independent passivity, which is present in a wide range of physical systems, we propose structured neural-PI controllers that have provable guarantees on stability and zero steady-state output tracking error. If communication between neighbours are available, we further extend the controller to distributedly achieve optimal resource allocation at the steady-state. We explicitly characterize the stability conditions and engineer neural networks that satisfy them by design. Experiments on traffic and power networks demonstrate that the proposed approach can improve both transient and steady-state performances compared to existing state-of-the-art, while unstructured neural networks lead to unstable behaviors. 


# Language and Dependencies
All code are implemented in Python.  We used the open-source Python package Tensorflow 2.0 to implement RNN and train the neural networks. Data for the power system is imported from MATLAB as 'IEEE_39bus_Kron.mat'. 

