# Segfault Computing Cluster

Use [Segfault](https://www.thc.org/segfault) voluntary users resources to build a massive computing cluster.

## Idea

The main idea is to create what is called a [Boewulf cluster](https://en.wikipedia.org/wiki/Beowulf_cluster) using the resources given by voluntary users from the [Segfault](https://www.thc.org/segfault) platform.

It would need a main node to manage all clients that would connect to it and form a massive computing cluster where ones could run heaving computing tasks shared across voluntary users nodes.

## Stack

I'll try to describe here more in details how the main node should be implemented and software will be required to install.

### Main Node

On the main node, the following will be have to be installed:

* [SLURM](https://en.wikipedia.org/wiki/Slurm_Workload_Manager)
* [MPICH](https://en.wikipedia.org/wiki/MPICH) or [Open MPI](https://en.wikipedia.org/wiki/Open_MPI)
* [Stunnel](https://www.stunnel.org/)
* [Nginx](https://en.wikipedia.org/wiki/Nginx)
* [PHP](https://www.php.net/) / [PHP-FPM](https://www.php.net/manual/en/book.fpm.php)
* [MUNGE](https://dun.github.io/munge/)

### Admin Node

The admin node will be used to control the main node.

### Client Nodes

The client nodes will connect to the main node and form the massive computing cluster. The more clients connected, the bigger the cluster get.

## References

* https://en.wikipedia.org/wiki/Beowulf_cluster
* https://en.wikipedia.org/wiki/Slurm_Workload_Manager
* https://en.wikipedia.org/wiki/MPICH
* https://en.wikipedia.org/wiki/Open_MPI
* https://slurm.schedmd.com/
* https://slurm.schedmd.com/quickstart.html
* https://slurm.schedmd.com/quickstart_admin.html
* https://slurm.schedmd.com/tutorials.html
* https://slurm.schedmd.com/configless_slurm.html
* https://slurm.schedmd.com/network.html
* https://slurm.schedmd.com/containers.html
* https://slurm.schedmd.com/mpi_guide.html
* https://slurm.schedmd.com/configurator.html
* https://slurm.schedmd.com/configurator.easy.html
* https://slurm.schedmd.com/rest.html
* https://slurm.schedmd.com/rest_api.html
* https://slurm.schedmd.com/slurmrestd.html
* https://dun.github.io/munge/
* https://github.com/dun/munge/wiki/Installation-Guide