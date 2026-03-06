⚡ H-Inf FuelCell: Robust Aviation Energy Management

Optimal H infinite control to prevent Oxygen Starvation in Hydrogen-powered aircraft.
🌪️ The Problem
Hydrogen fuel cells are fragile. If you draw too much power too fast (like during takeoff), the "Oxygen Excess Ratio" crashes. 
If this happens for even a few seconds, the membrane is ruined. To make things harder, the air is thinner at 10,000ft, which changes the system dynamics completely.

🛡️ The Robust SolutionThis project implements an H infinite Regulator. 
Unlike basic controllers, this math assumes the "worst-case" scenario.Altitude Agnostic: Designed to handle 30% variations in air density and compressor aging. 
✈️Gamma-Performance: We use the L2 gain bound gamma  to ensure that even a massive power spike (Disturbance w) has a minimal impact on Oxygen Pressure (Output z).
📉Real-Time Ready: The control law is a simple matrix multiplication u = -Kx, making it lightning-fast for embedded flight computers. 🚀
