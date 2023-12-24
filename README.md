# simulate-oscilloscope
simulate oscilloscope
# Code for Simple Oscilloscope Simulation
import numpy as np
import matplotlib.pyplot as plt

def simulate_oscilloscope():
    # Generate a sine wave for simulation
    frequency = 1  # in Hertz
    amplitude = 1
    sampling_rate = 1000  # in samples per second
    time = np.arange(0, 1, 1 / sampling_rate)
    signal = amplitude * np.sin(2 * np.pi * frequency * time)

    # Plot the simulated signal
    plt.plot(time, signal)
    plt.title("Oscilloscope Simulation")
    plt.xlabel("Time (seconds)")
    plt.ylabel("Amplitude")
    plt.show()

# Example usage
simulate_oscilloscope()
