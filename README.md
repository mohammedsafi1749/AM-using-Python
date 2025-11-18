## EXP NO: 5 AM-using-Python
Amplitude Modulation and Demodulation using NumPy and Matplotlib

## Aim:
To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. 

## Apparatus :

                Software: Python with NumPy and Matplotlib libraries
                Hardware: Personal Computer

## Theory:


Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting
information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of
the message signal. The general form of an AM signal is:

## Algorithm:

         1. Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
         
         2. Generate Time Axis: Create a time vector for the signal duration.
         
         3. Generate Message Signal: Define the message signal as a cosine wave
         
         4. Generate Carrier Signal: Define the carrier signal as a cosine wave.
         
         5. Modulate Signal: Apply the AM formula to obtain the modulated signal
         
         6. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.
         

## Program:

    import numpy as np
    import matplotlib.pyplot as plt
    Am = 20.3
    fm = 394
    Ac = 204.6
    fc = 3940
    fs = 39400
    t = np.arange(0, 2/fm, 1/fs)
    m = Am * np.cos(2 * np.pi * fm * t)
    c = Ac * np.cos(2 * np.pi * fc * t)
    s = (Ac + m) * np.cos(2 * np.pi * fc * t)
    plt.subplot(3,1,1)
    plt.plot(t, m)
    plt.subplot(3,1,2)
    plt.plot(t, c)
    plt.subplot(3,1,3)
    plt.plot(t, s)

## Output Waveform:
<img width="554" height="413" alt="download" src="https://github.com/user-attachments/assets/fbfc8b73-f563-4f8a-a965-c55d8eac6a65" />

## Tabular Column:
![WhatsApp Image 2025-10-15 at 13 10 26_d5b46a54](https://github.com/user-attachments/assets/04cdf74b-8eb7-44ff-bd39-d5be7745cda8)

## Result:

The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots.
Thus AM is implemented using numPy and Matplotlib.
