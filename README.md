### NTU's aggressive kernel patch set

Some of these patches should not be used, you have been warned.

Boot params for best latency: 

nohz_full=1,2,3 rcu_nocbs=1,2,3 isolcpus=1,2,3 idle=poll

For a good mix of latency and system performance:

nohz_full=1,2,3 rcu_nocbs=1,2,3 idle=poll

Leaving isolcpus off allows you to use all 4 cores for non-RT tasks.
