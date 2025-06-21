# COSSIM-HPC
This is the COSSIM [1] extension which is developed to simulate complete heterogeneous HPC Systems supporting ARM and RISC-V CPUs.

## The contribution of this work can be summarized in the following points:
- The first known open-source integrated simulation framework which can simulate complete heterogeneous HPC Systems supporting Full System ARM and RISC-V architectures.
- The integration of PCI Host to RISC-V GEM5 board and adaptation of GEM5 ethernet card to it to simulate multi-node RISC-V systems in the COSSIM simulator (we merge the development code in the official GEM5 repository).
- An innovative flow to enable the designers to simulate the complete aspects of HPC Systems (i.e. CPU and Network Environment) through real MPI applications within one simulation framework.
- The integration of VEF traces Framework [2] to analyze communication traffic of MPI-based applications and generate traffic traces that can be used to feed other network simulator tools.
- The use of VEF traces generated with COSSIM-HPC (using ARM and RISC-V processors) to feed the SAURON network simulator, which models the InfiniBand and BXI network technologies.


## Execution
We have created a Virual Machine which we have install everything there. You may donwload it from [here](https://ihuedu-my.sharepoint.com/:f:/g/personal/ntampouratzis_ihu_gr/EpgTQ8xY-FtHgnLzDxYJCtQBNnVsaTyawzHqjFu7B8lxIA?e=eVKroj) (It is tested using VMWare 16.1 tools - [download the VM tools for Windows from here](https://ihuedu-my.sharepoint.com/:u:/g/personal/ntampouratzis_ihu_gr/EceCqMJ2-QdOpL3wbKX7bW8BZAuX1MzVrEpsxS9IpzNXJw?e=9HiYY4)). The VM password is <b>redsea1234</b> .

You may see the related video for instructions [MPI-on-COSSIM-multinode](https://ihuedu-my.sharepoint.com/:v:/g/personal/ntampouratzis_ihu_gr/ESUBDBEs3n9Jt0sJ9vCBqaoBVIqRlWH1ql45P6MrVsPmMg). 

## References
<a id="1">[1]</a> 
N. Tampouratzis, I. Papaefstathiou, A. Nikitakis, A. Brokalakis,
S. Andrianakis, A. Dollas, M. Marcon, and E. Plebani, “A novel,
highly integrated simulator for parallel and distributed systems,”
ACM Trans. Archit. Code Optim., vol. 17, no. 1, Mar. 2020.
Available: https://dl.acm.org/doi/10.1145/3378934

<a id="2">[2]</a> Andújar, F.J., Sánchez de la Rosa, M., Escudero-Sahuquillo, J. et al. Extending the VEF traces framework to model data center network workloads. J Supercomput 79, 814–831 (2023). https://doi.org/10.1007/s11227-022-04692-0
