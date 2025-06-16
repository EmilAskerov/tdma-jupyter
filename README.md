# TDMA jupyter
A distributed system is described by the following reaction-diffusion equations:

dx/dt = A - (B + 1) * x + x^2 * y + D_x * ∆x^2

dy/dt = Bx - x^2 * y + D_y * ∆y^2

The model was numerically implemented using an operator splitting technique, where the reaction kinetics were solved using a fourth-order Runge-Kutta scheme, and the diffusion terms were handled by the Tridiagonal Matrix Algorithm (TDMA, or Thomas algorithm).

Turing structures were obtained for the parameter set: D_x = 1, D_y = 10, A = 3, and B = 7.5.

The system domain size was L ≈ 50, chosen in conjunction with zero-flux (Neumann) boundary conditions, simulating impermeable walls.

Conservative boundary conditions were employed in the TDMA scheme for the diffusion components achieving second-order accuracy for the spatial discretization.

Tested using VSCode and Python 3.13.3.
