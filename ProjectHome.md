This python tool reads LIGGGHTS (http://www.liggghts.com) local dump files containing particle contact data and produces a VTK file for visualising contact chains and networks.

The visualisation is done simply by connecting the centres of particles in contact with a VTKLine which is coloured by the magnitude of the force.

Later versions will deal better with periodic boundaries, and potentially use cylinders instead of lines such that the radius of the cylinder is scaled by the force magnitude.

PyEVTK is currently required to generate binary VTK files: https://bitbucket.org/pauloh/pyevtk

Future versions will fall back to a basic ASCII VTK file if this PyEVTK is not found.