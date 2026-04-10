# Artificial Pancreas

## 📌 Description

This project analyzes an artificial pancreas system that automatically regulates blood glucose levels using a closed-loop control system.

---

## ⚙️ Working Principle

1. Glucose measurement  
2. Error calculation  
3. Insulin dose determination  
4. Insulin delivery  
5. Feedback loop  

---

## 🧮 Minimal Model

dG/dt = -(SG + x)G + C  
dx/dt = kaI - kb x  

Operating point: (7.5, 0.009, 15)

---

## 📉 Linearized Model

dx1/dt = -0.023x1 - 7.5x2  
dx2/dt = 6·10^-6 u - 0.01x2  

---

## 🎛️ Controller

A PID controller is used:  
Gr(s) = kd s² + kp s + ki  

Parameters:  
Kd = -711  
Kp = -24.9  
Ki = -0.2  

---

## ✅ Stability

The system is stable (Nyquist analysis).

