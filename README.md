# pysf
Extremely simple python spaceflight simulation.
This script is a 2D orbital mechanics simulator built using Pygame. It features a dual-body gravity system (Earth and Moon), real-time trajectory prediction, and time-dilation controls. It is designed for testing orbital maneuvers such as reaching stable orbits or performing lunar flybys.

System Controls

W triggers main thrusters to accelerate the craft forward.

A and D rotate the craft left and right to adjust heading.

M toggles between Ship View (close-up) and Map Mode (wide-scale orbital view).

Period (.) increases the time-warp speed up to 1024x.

Comma (,) decreases the time-warp speed down to 1x.

CTRL + B performs a "Quick-Load" to revert the craft and moon to their state from 600 frames ago.

Mouse Wheel adjusts the zoom level while in Map Mode.

Features

Gravity Model: Uses an inverse-square law calculation for Earth. The Moon has a defined Sphere of Influence (SOI); gravity from the Moon only affects the craft when it enters this radius.

Trajectory Prediction: Draws a projected path showing where the craft will travel based on current velocity. It highlights the Apogee (highest point) in red and the Perigee (lowest point) in cyan.

Atmosphere: A visual indicator for Earth's atmosphere is provided, though drag physics are currently simplified.

Landing Logic: If the craft touches Earth's surface, velocity and angular momentum are reset to zero to simulate a touchdown or impact.
