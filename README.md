# Handling-Signal-Distortion

------------------------------------

In the realm of Internet of Things (IoT), a critical application involves the continuous monitoring of temperature in various locations using dedicated sensors. These sensors record temperature values over time, but due to hardware constraints, their memory must be periodically cleared. This is achieved by transmitting the stored values to a central base unit. The recorded temperature values, denoted as x[n], are, however, subject to blur distortions and additive noise during transmission to the base unit.

The blur distortion is modeled by a system with an impulse response, h[n] = [1, 4, 6, 4, 1] (with the center value of 6/16 corresponding to n = 0). Consequently, the received signal at the base unit is represented as y[n].

The task at hand is to develop two distinct approaches to recover the original temperature signal x[n] from the distorted signal y[n]. The two approaches are as follows:

1. **Remove Noise First, Then Sharpen (Deblur)**
2. **Sharpen (Deblur) First, Then Remove Noise**

After implementing both approaches, a critical analysis is required to compare x1[n] and x2[n] with the original signal x[n]. This comparative analysis aims to draw conclusions regarding the efficacy of each approach in recovering the true temperature values from the distorted signals.
