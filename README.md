Optimized Satellite Position and Signal Strength Simulation

Functions
1. simulate_orbit(t, orbital_radius)
   Simulates the position of a satellite in orbit over time. The satellite follows a circular orbit at a specified radius, and its position is determined by the angle of rotation as a function of time.

2. signal_strength(distance, interference_factor)
   Computes the signal strength based on the distance between the satellite and the ground station. The strength is modeled as an inverse square law, with an additional interference factor based on distance.

3. optimize_signal(params)
   A function used for optimization, which calculates the signal strength for a given satellite position. The function returns the negative of the strength to be minimized using the minimize function from SciPy.

Variables
- earth_radius: The radius of the Earth in kilometers (6371 km).
- geo_orbit_radius: The radius of the geostationary orbit (42164 km, which includes Earth's radius and the altitude of the geostationary orbit).
- signal_speed: The speed of the signal, set to the speed of light (3e8 m/s).
- initial_position: The initial position of the satellite for optimization, set to the geostationary orbit radius along the x-axis.
