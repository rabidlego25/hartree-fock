# An Application of Self-Consistent Fields (SCF) and Mean-Field Theory (MFT)

**Author:** Austin Tabb

# An Application of Self-Consistent Fields (SCF) and Mean-Field Theory (MFT)

**Author:** Austin Tabb

---

### Many-Body Systems

Physicists have long sought to characterize observable phenomena with fundamental units such as energy, position, and time. Using these fundamental units, physicists construct coherent mathematical frameworks that reconcile observed phenomena with logical derivations. Much of early classical physics was constructed through this lens. Oftentimes, physicists opt to understand a compilation of observed phenomena. Rather than looking at one particle defined by fundamental units, one may want to understand $N$ particles, each also characterized by fundamental units. Each particle may be subject to various interacting terms, meaning the existence of one particle may influence the characterization of others through a coherent mathematical framework. This is referred to as a self-consistent many-body system.

Understanding many-body systems is complex and has drawn scientists from various fields—computer science, mathematics, and chemistry. Materially, most systems rely on some degree of many-body analysis. Any physical tool in reality is fundamentally caricatured by many-body dynamics. These dynamics are further complicated by the intricacies of quantum mechanics. These notes focus on early approaches to self-consistent methods and mean-field theories—the solutions and methods of which have vast implications on our understanding of thermodynamic systems and variables such as entropy and free energy.

#### The Hamiltonian and the Many-Body Dilemma

The crux of the problem begins with the classical Hamiltonian. Given a $N_{\text{nuclei}}$-atom system with $N$ electrons, assuming the nuclei contain charges $Z_1e, \dots, Z_{N_{\text{nuclei}}}e$ at positions $R_1, \dots, R_{N_{\text{nuclei}}}$ and the electrons are at positions $r_1, \dots, r_N$, the Hamiltonian is:

$$
\hat{H} = -\frac{\hbar^2}{2m}\sum_{i=1}^N \nabla_{i}^2 
+ \frac{1}{4\pi\epsilon_0}\left(\sum_{I<J=1}^{N_{\text{nuclei}}}\frac{Z_I Z_J e^2}{|\vec{R_I}-\vec{R_J}|}
- \sum_{i=1}^{N}\sum_{I=1}^{N_{\text{nuclei}}}\frac{Z e^2}{|\vec{r_i}-\vec{R_I}|}
+ \sum_{i<j=1}^{N}\frac{e^2}{|\vec{r_i}-\vec{r_j}|}\right)
$$
