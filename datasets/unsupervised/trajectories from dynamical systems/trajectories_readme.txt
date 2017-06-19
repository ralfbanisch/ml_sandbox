These datasets are all generated from a discrete-time or continuous time dynamics.
What can you find out about the dynamics? Can you learn, for example, the equations
of motion? Can you find structure (fixed points, attractors, (almost) invariant sets)?

In all of these datasets, different columns correspond to different observables (e.g. x, y, z, x^2,...)
while different rows correspond to different time points. The exception is the
'molecule2' dataset (see below). The first column is usually time.

The 'labels' folder contains (at least partially) labelled data. henon1.csv etc. are
realizations of the Henon Map. The two rows correspond to 'xn' and 'yn', respectively.
The parameters are different for each realization and unknown. lorenz1.csv etc.
has realizations of the famous Lorenz system. The rows are 'time', 'x', 'y', 'z'.
The parameters are also unknown.

The 'no labels' folder contains various unlabelled datasets. The amount of information
given varies. In 'dynamics1_full.csv', the system is 3D and all three coordinates are
given as observations. The columns are 'time', 'x', 'y', 'z'. In 'dynamics2_partial.csv',
only the columns 'time' and 'x' are given but the dynamics is 3D.

'molecule1.csv' is a molecular dynamics example. The columns correspond to the 3D
coordinates of the heavy atoms of the molecule, in the format 'x1', 'y1', 'z1', 'x2', 'y2', ...
Heavy atoms are all non-hydrogen ones. The full dynamics here has hundreds of
degrees of freedom due to the surrounding water bath, but only 12 coordinates are given.
