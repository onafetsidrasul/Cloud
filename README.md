# Cloud Basic
## VMs cluster
The project start considering a VMs cluster of 3 machines: a master and 2 nodes.
## Benchmark
Several benchmarks are executed: HPCC, sysbench, IOZone and iperf.
To really stress the setup sysbench is executed also simultaneously with HPCC as IOZone with iperf.
## Docker cluster
After this a very similar Docker cluster is created and tested.
## Benchmark and comparison
The benchmarks carried on in this case are sysbench, IOZone and iperf.
# Cloud Advanced
## Namespace creation
The second project starts with the creation of 2 network namespaces.
## Namespace connection
At this point the 2 namespaces are connected via veth pair, via 2 veth pairs and a bridge, and via 2 veth pairs, 2 bridges and a vxlan tunnel.
## Benchmark
The benchmark is carried on using iperf.
## Kubernetes cluster
The last part is about the creation of a Kubernetes cluster on the previous used Vms cluster. For this purpose each machine has a pod that can communicate with its peers.
## Benchmark and Kube-Prometheus stack
The benchmark carried on in this case is HPCC with the focus on hpl. The cluster can be monitored using the Kube-prometheus stack.
