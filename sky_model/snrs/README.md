# Supernova remnants

This folder contains a synthetic population of supernova remnants.

From "Pierre V. Cristofari" <pc2781@columbia.edu>

We rely on a simple Monte Carlo approach to simulate the population of SNRs potentially detectable by CTA. 
We simulate the time and location of supernova explosions in the Galaxy, assuming a rate of 3 SN per century, and a spatial distribution described as in Faucher-Giguere & Kaspi 2006. Two mechanisms, via four types of progenitors, are considered:~thermonuclear (type Ia) and core--collapse (types Ib/c, IIP, IIb). The relative rates and typical parameters associated to each type, such as the total supernova explosion energy, the velocity of the wind and the mass of the ejecta, are adopted as in Ptuskin et al. 2010, so that every simulated supernova is assigned a type and corresponding parameters. 
At the location of each supernova, the typical value of the interstellar medium (ISM) is derived from surveys of atomic and molecular hydrogen as given in Nakanishi & Sofue 2003. The evolution of the shock radius R_sh and velocity u_sh is computed using analytical and semi--analytical description of Chevalier 1982, Ptuskin & Zirakashvili 2005.  

Finally, the gamma--ray luminosity of each SNR is computed. The contribution of protons and electrons is taken into account. At the shock, the particles are assumed to be accelerated with a slope following a power--law in momentum n(p) = p^{-\alpha}, where alpha is treated as a parameter in the range 4.1 - 4.4. At the shock, we assumed that a fraction xi_CR of the ram pressure of the shock expanding through the ISM is converted into CR, and the shock compression factor is $\sigma=4$.  

We follow by computing the leptonic component. 
The spectrum of electrons is parametrized adopting the same spectral shape as protons $\propto p^{-\alpha}, weighted by a factor K_ep, for momenta p < p_break, where p_break accounts for radiative losses. above p_break the electron spectrum steepens by one order and follows p^{-\alpha-1}. The maximum momentum of electrons is reached when the synchrotron loss time is of the order of the acceleration rate. The gamma--ray luminosity from inverse Compton scattering of electrons on the cosmic microwave background is computed following the description proposed by Blumenthal & Gould 1970

The approach presented here is described more in detail in Cristofari et al. 2013,2017 and was used to provide a statistical test for the SNR hypothesis of the origin of CRs. 



The following files correspond to results of a single Monte-Carlo trial:  


*_1.txt takes a cosmic ray efficiency xi_CR = 0.1 and alpha = 4.25 
*_2.txt takes a cosmic ray efficiency xi_CR = 0.05 and alpha = 4.25 



We use version "_2" for 1DC
