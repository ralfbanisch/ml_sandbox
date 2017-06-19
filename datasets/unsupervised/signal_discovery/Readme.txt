These images contain signal areas (non-zero/black) and noise-free non-signal areas (zero/white). Add gaussian noise to each pixel and try to tell apart noise from signal in an unsupervised fashion (i.e. do not use an classification algorithm and your ground truth knowledge!). Compare to ground truth. How robust is your algorithm to increasing the noise level?
Hints:
- Try to estimate a denoised version of the image with the help of a sparsity-enforcing regularizer (L1-regularizer)
- It could help to use adjacency information of the pixels: if one pixel contains signal (non-signal), its neighbour is more likely to contain signal (non-signal) as well. Can you derive a regularizer from this idea?

Find a parametrization of your algorithm that allows to tune for more vs. less pixels being identified as signal.

Once your algorithm is working, try it on a real dataset. An interesting fMRI dataset you will find at https://openfmri.org/dataset/ds000051/. We recommend "datasets/openfmri.org_ds051/sub010/BOLD/task001_run001/bold.nii.gz", which is indexed by one time and three space coordinates.
You can load the fMRI data using e.g. the nibabel library for Python. 
