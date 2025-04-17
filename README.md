# Analog Signal Modulation Simulator
An interactive web-based simulator for visualizing different signal modulation techniques: Amplitude Modulation (AM), Frequency Modulation (FM), and Phase Modulation (PM).
📝 Table of Contents

Overview:
Features
Demo
Technical Details
Mathematical Implementation
How to Use
Installation
Contributors
License

🔭 Overview
The Signal Modulation Simulator is an educational tool designed to help students and enthusiasts understand the fundamental concepts of signal modulation techniques. It provides a real-time visualization of how carrier signals are modulated by message signals using different methods:

Amplitude Modulation (AM): Changes the amplitude of the carrier wave
Frequency Modulation (FM): Changes the frequency of the carrier wave
Phase Modulation (PM): Changes the phase of the carrier wave

By manipulating various parameters, users can observe the effects on the resulting modulated signal and gain intuitive understanding of these important communication concepts.
✨ Features

Real-time Visualization: See the message signal, carrier signal, and modulated signal update in real-time
Interactive Controls: Adjust parameters like:

Carrier amplitude and frequency
Message amplitude and frequency
FM sensitivity (Kf)
PM sensitivity (Kp)


Educational Explanations: Learn about each modulation technique with mathematical formulas and descriptions
Parameter Guidance: Get recommendations for optimal parameter settings for each modulation type
Visual Indicators: Warning indicators when parameters might create artifacts
Responsive Design: Works on desktop and mobile devices
Play/Pause & Reset Controls: Control the simulation at your own pace

🎮 Demo
Check out the live demo: Signal Modulation Simulator Demo
🔧 Technical Details
This project is built entirely with vanilla front-end technologies:

HTML5: Structured semantic markup for the application
CSS3: Modern styling with flexbox layout, CSS variables, gradients, and animations
JavaScript: Canvas API for drawing waveforms and managing simulation state
No Dependencies: Zero external libraries or frameworks

The waveforms are rendered using the HTML5 Canvas API, with mathematical calculations performed in real-time to generate accurate representations of each signal type.

📊 Mathematical Implementation

The simulator implements the following mathematical equations for each modulation type:

Amplitude Modulation (AM)
x_AM(t) = A_c × (1 + μ × cos(2π × f_m × t)) × cos(2π × f_c × t)
where μ = A_m/A_c is the modulation index.

Frequency Modulation (FM)
x_FM(t) = A_c × cos(2π × f_c × t + β × sin(2π × f_m × t))
where β = (K_f × A_m)/f_m is the modulation index.

Phase Modulation (PM)
x_PM(t) = A_c × cos(2π × f_c × t + K_p × m(t))
where m(t) = A_m × cos(2π × f_m × t) is the message signal.


📖 How to Use

Select a modulation type from the dropdown menu (AM, FM, or PM)
Adjust the parameters using the sliders:

Carrier Amplitude (Ac): Controls the height of the carrier signal
Message Amplitude (Am): Controls the height of the message signal
Carrier Frequency (fc): Controls how many cycles of the carrier signal occur per second
Message Frequency (fm): Controls how many cycles of the message signal occur per second
FM Sensitivity (Kf): (For FM only) Controls how much the frequency changes
PM Sensitivity (Kp): (For PM only) Controls how much the phase changes


Click "Start Simulation" to begin the animation
Use "Reset" to reset the time parameter
Observe the waveforms and how changes in parameters affect the modulated signal

🚀 Installation

Clone the repository:

bashgit clone https://github.com/AyushBhatnagar10/Analog-Signal-Modulation.git

Navigate to the project directory:

bashcd Analog-Signal-Modulation

Open the AM,PM,FM.html file in your browser:

bash# On macOS
open AM,PM,FM.html

# On Windows
start AM,PM,FM.html

# On Linux
xdg-open AM,PM,FM.html
No build tools or additional dependencies are required!


👥 Contributors

Ayush Bhatnagar (23BTM007)
Jenil Buha (23BCE039)

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

Made with ❤️ as part of an educational project on signal processing and communications engineering.
