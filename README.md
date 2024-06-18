# Efficient-Recurrent-Real-Video-Restoration

This GitHub is associated to the following article:

A. Buades, J.L. Lisani, Efficient Recurrent Real Video Restoration, submitted to Digital Signal Processing, 2024
Preprint: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4442784

The GitHub contains a dataset of video sequences used to study the behaviour of the proposed processing chain for the removal of such degradations as blur, flicker, correlated noise, tonal changes and low contrast in real video sequences.

The original sequences were obtained by cropping portions (simulating a panning motion) of the noise-free images available at http://mcolom.info/pages/no_noise_images/. These original sequences can be found in the **cleandata** folder.

All the sequences consist of 20 frames, five of which were blurred by convolution with some of the kernels described in [1] and implemented in https://ipolcore.ipol.im/demo/clientApp/demo.html?id=211. 

Correlated noise was produced by blurring (with a Gaussian kernel of standard deviation 1.2) a zero-mean white Gaussian noise image with noise level $\sigma$ (with $\sigma$ in {10, 20}) that was added to each frame of the sequences. These noisy sequences can be found in the **bnoisy** folder (the number at the end of the subfolder names indicates the amount of added noise).

A last test set was obtained by first modifying the original sequences to simulate a tonal change, and applying the same noise and blurring process described above. These sequences can be found in the **tbnoisy** folder (the number at the end of the subfolder names indicates the amount of added noise).

[1] Levin, Anat, Yair Weiss, Fredo Durand, and William T. Freeman. "Understanding and evaluating blind deconvolution algorithms." In 2009 IEEE conference on computer vision and pattern recognition, pp. 1964-1971. IEEE, 2009.

For more information please contact joseluis.lisani@uib.es

**License**: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
