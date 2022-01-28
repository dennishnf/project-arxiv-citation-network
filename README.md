[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.png)](https://www.python.org/)
[![MIT Licence](https://img.shields.io/badge/License-MIT-blue.png)](https://opensource.org/licenses/mit-license.php)
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.png)](https://github.com/dennishnf/project-arxiv-citation-network/issues)
[![Open Source Love](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-1abc9c.png)](https://github.com/dennishnf/project-arxiv-citation-network/)
[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Download%20and%20use%20the%20Project:%20ArXiv%20Citation%20Network&url=https://github.com/dennishnf/project-arxiv-citation-network&hashtags=network,arxiv,citations,networkx)    


# Project ArXiv Citation Network

## Overview

This project involved the analysis of the ArXiv citation network.


## Data

The data was extracted from: [https://github.com/mattbierbaum/arxiv-public-datasets/releases/tag/v0.2.0](https://github.com/mattbierbaum/arxiv-public-datasets/releases/tag/v0.2.0). More exactly, we'll use the file "internal-references-v0.2.0-2019-03-01.json.gz", which contains the list of papers and their references, all papers using their arXiv IDs.


## Results


### Citation Network using NetworkX

<p align="center">
<img src=".images-readme/citation_network.png" alt="image" width="700"/>
</p>


### In-degree and Out-degree analysis

<p align="center">
<img src=".images-readme/in_degree_distribution.png" alt="image" width="350"/>
<img src=".images-readme/out_degree_distribution.png" alt="image" width="350"/>
</p>

<p align="center">
<img src=".images-readme/in_degree_distribution_loglog.png" alt="image" width="350"/>
<img src=".images-readme/out_degree_distribution_loglog.png" alt="image" width="350"/>
</p>

<p align="center">
<img src=".images-readme/in_degree_distribution_fitted.png" alt="image" width="350"/>
<img src=".images-readme/out_degree_distribution_fitted.png" alt="image" width="350"/>
</p>


### Table of Centralities

The most important centrality is PageRank, because this measure uncovers nodes whose influence extends beyond their direct connections into the wider network.

<p align="center">
<img src=".images-readme/centralities_table.png" alt="image" width="800"/>
</p>


### Top 10 influencial papers in arXiv based on PageRank Centrality

Top 1 , Id arXiv: 1705.11098 , Centrality: 0.0024     
Title: Modified Gravity Theories on a Nutshell: Inflation, Bounce and Late-time  Evolution 

Top 2 , Id arXiv: 1812.00847 , Centrality: 0.0023     
Title: Rescuing Quartic and Natural Inflation in the Palatini Formalism 

Top 3 , Id arXiv: 1811.09514 , Centrality: 0.002     
Title: Higgs inflation in the Palatini formulation with kinetic terms for the  metric 

Top 4 , Id arXiv: 1501.05671 , Centrality: 0.002     
Title: Resurgence and the Nekrasov-Shatashvili Limit: Connecting Weak and  Strong Coupling in the Mathieu and Lam'e Systems 

Top 5 , Id arXiv: 1607.01001 , Centrality: 0.0019     
Title: Dark Matter from a Classically Scale-Invariant $SU(3)_X$ 

Top 6 , Id arXiv: 0710.4947 , Centrality: 0.0018     
Title: Physics at a future Neutrino Factory and super-beam facility 

Top 7 , Id arXiv: 1812.11159 , Centrality: 0.0018     
Title: Spatially modulated and supersymmetric deformations of ABJM theory 

Top 8 , Id arXiv: 1802.10257 , Centrality: 0.0016     
Title: The correlation of extragalactic $\gamma$-rays with cosmic matter  density distributions from weak-gravitational lensing 

Top 9 , Id arXiv: 1502.02866 , Centrality: 0.0016     
Title: The nature of the Diffuse Gamma-Ray Background 

Top 10 , Id arXiv: 1901.11298 , Centrality: 0.0016     
Title: Non Unitarity at DUNE and T2HK with Charged and Neutral Current  Measurements 


### Field Category Network using NetworkX

<p align="center">
<img src=".images-readme/fields_network_networkx.png" alt="image" width="700"/>
</p>


### Field Category Network using Cytoscape

<p align="center">
<img src=".images-readme/fields_network_cytoscape.png" alt="image" width="700"/>
</p>



## References

- Clement, C. B., Bierbaum, M., O’Keeffe, K. P., & Alemi, A. A. (2019). On the Use of ArXiv as a Dataset. arXiv [cs.IR]. Opgehaal van http://arxiv.org/abs/1905.00075

- Clauset, A., Shalizi, C. R., & Newman, M. E. J. (2009). Power-Law Distributions in Empirical Data. SIAM Review, 51(4), 661–703. doi:10.1137/070710111

- Page, L., Brin, S., Motwani, R., & Winograd, T. (1998). The PageRank Citation Ranking: Bringing Order to the Web.




<!---

git pull
git add -A
git commit -m "updating readme"
git push -u origin main

--->