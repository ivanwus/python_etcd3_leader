# python_etcd3_leader
Sample for python-etcd3 API to find out the etcd cluster leader

# etcd command line client to check cluster status
<pre><code>  export ETCDCTL_API=3
  HOST_1=10.1.1.11
  HOST_2=10.1.1.12
  HOST_3=10.1.1.13
  ENDPOINTS=$HOST_1:2379,$HOST_2:2379,$HOST_3:2379
  etcdctl --endpoints=$ENDPOINTS member list
  etcdctl --write-out=table --endpoints=$ENDPOINTS endpoint status
</code></pre>

# Configuration and environment
| project | version | link |
| :---         |     :---:      |    :--- |
| etcd   | 3.2.25     | https://github.com/etcd-io/etcd    |
| python-etcd3     | 0.8.1       |  https://github.com/kragniz/python-etcd3    |

# Reference
https://coreos.com/etcd/docs/latest/demo.html  
https://python-etcd3.readthedocs.io/en/latest/usage.html  
https://www.sandtable.com/etcd3-leader-election-using-python/  
