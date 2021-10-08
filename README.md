In normal situation of MPTCP with the same bandwidth in all paths, uncoupled BBRv1
in MPTCP mainly improves its rates in the total of all the paths, but when one path
is congested the performance of uncoupled BBR1 gets lower, because of the out of order
problem.
We have proposed a method to resolve this problem, the amelioration is based on the
normal version of BBRv1, to achieve the goal of all subows congestion windows receives
in one time, we have reduced the congestion window in the high congested path to make
the delay of transmission lower than before and equal to the delay of transmission the
data in the less congested subows to let all the congestion windows arrive the destination
in the same time and the acknowledgment of the global window is sent.

#Instructions:

How to Run:

Just compile and install is as a module. Change the default Congestion Algorithm to "NCG_C-MPBBR"

Above development was based on the MPTCP v0.95.0 deployed in Linux kernel version of v4.19.206 


Regards,

Computer Systems Enginner Drici Oussama.

For any information contact me at o.drici@esi-sba.dz

