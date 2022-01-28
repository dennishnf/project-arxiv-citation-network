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