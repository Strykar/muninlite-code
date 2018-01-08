# Cloned from https://sourceforge.net/projects/muninlite/
Added plugins:
1. time/ntp{date,dispersion,jitter,offset,stratum,wander} plots using 'ntpq -c rv' and not the deprecated ntpdate. Tested on ntpsec-1.0.1/ntpd-4.2.8p10 on OpenWrt SNAPSHOT r5638-0f72690a2d, inspired by https://www.wraith.sf.ca.us/ntp/do-ntp-rrdstats   
2. sensors/apu{power,temp} to plot PC Engine's APU2c4 AMD GX412-TC CPU and Phison mPCI-e mSATA SSD temps

TODO: Use ntpd statistic files {clock,loop,peer}stats to plot local clock/frequency offsets and refclock/peer jitter instead of ntpq
