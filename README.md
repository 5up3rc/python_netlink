###此库主要实现了内核netlink, ioctl的通信接口, 现在正在开发中
###取得当机的tcp连接信息
```shell
python sock_diag.py
SRC                           DST                           R/W QUEUE           STATE               
127.0.0.1:631                 0.0.0.0:0                     0/128               LISTEN              
127.0.0.1:25                  0.0.0.0:0                     0/100               LISTEN              
0.0.0.0:17500                 0.0.0.0:0                     0/128               LISTEN              
172.16.0.2:42653            103.110.162.115:80              0/0                 ESTABLISHED         
172.16.0.2:57302            210.151.124.12:80               0/1                 SENT   
```

###示例取得网卡接口的信息
```shell
python if.py 
{'address': '\xd1\xde\x9bv\\\xee',
 'af_spec': {'cacheinfo': {'max_reasm_len': 65535,
                           'reachable_time': 43468,
                           'retrans_time': 1000,
                           'tstamp': 9508953},
             'conf': {'accept_dad': 1,
                      'accept_ra': 1,
                      'accept_ra_defrtr': 1,
                      'accept_ra_pinfo': 1,
                      'accept_ra_rt_info_max_plen': 0,
                      'accept_ra_rtr_pref': 1,
                      'accept_redirects': 1,
                      'accept_source_route': 0,
                      'autoconf': 1,
                      'dad_transmits': 1,
                      'disable_ipv6': 0,
                      'force_mld_version': 0,
                      'force_tllao': 0,
                      'forwarding': 0,
                      'hoplimit': 64,
                      'max_addresses': 16,
                      'max_desync_factor': 600,
                      'mc_forwarding': 0,
                      'mtu6': 1500,
                      'ndisc_notify': 0,
                      'optimistic_dad': 0,
                      'proxy_ndp': 0,
                      'regen_max_retry': 3,
                      'rtr_probe_interval': 60000,
                      'rtr_solicit_delay': 1000,
                      'rtr_solicit_interval': 4000,
                      'rtr_solicits': 3,
                      'temp_prefered_lft': 86400,
                      'temp_valid_lft': 604800,
                      'use_tempaddr': 0},
             'icmp6stats': {'csumerrors': 0,
                            'inerrors': 0,
                            'inmsgs': 3,
                            'num': 6,
                            'outerrors': 0,
                            'outmsgs': 28},
             'stats': {'csumerrors': 0,
                       'fragcreates': 0,
                       'fragfails': 0,
                       'fragoks': 0,
                       'inaddrerrors': 0,
                       'inbcastoctets': 0,
                       'inbcastpkts': 0,
                       'indelivers': 3,
                       'indiscards': 0,
                       'inhdrerrors': 0,
                       'inmcastoctets': 1232678,
                       'inmcastpkts': 7585,
                       'innoroutes': 0,
                       'inoctets': 1232678,
                       'inpkts': 7585,
                       'intoobigerrors': 0,
                       'intruncatedpkts': 0,
                       'inunknownprotos': 0,
                       'num': 32,
                       'outbcastoctets': 0,
                       'outbcastpkts': 0,
                       'outdiscards': 2,
                       'outforwdatagrams': 0,
                       'outmcastoctets': 19536,
                       'outmcastpkts': 141,
                       'outnoroutes': 0,
                       'outoctets': 18220,
                       'outpkts': 125,
                       'reasmfails': 0,
                       'reasmoks': 0,
                       'reasmreqds': 0,
                       'reasmtimeout': 0},
             'token': {'part1': 0, 'part2': 0, 'part3': 0, 'part4': 0}},
 'boradcast': '\xff\xff\xff\xff\xff\xff',
 'carrier': 1,
 'group': 0,
 'ifname': 'wlo1',
 'linkmode': 1,
 'map': {'base_addr': 0,
         'dma': 0,
         'irq': 0,
         'mem_end': 0,
         'mem_start': 0,
         'port': 0},
 'mtu': 1500,
 'operstate': 6,
 'promiscuity': 0,
 'qdisc': 'mq',
 'rx_queues': 1,
 'stat64': {'mulicast': 0,
            'rx_bytes': 5385803085,
            'rx_compressed': 0,
            'rx_crc_errors': 0,
            'rx_dropped': 16,
            'rx_errors': 0,
            'rx_fifo_errors': 0,
            'rx_frame_errors': 0,
            'rx_length_errors': 0,
            'rx_missed_errors': 0,
            'rx_over_errors': 0,
            'rx_packets': 4057593,
            'tx_aborted_errors': 0,
            'tx_bytes': 277249054,
            'tx_carrier_errors': 0,
            'tx_compressed': 0,
            'tx_dropped': 0,
            'tx_errors': 0,
            'tx_fifo_errors': 0,
            'tx_heartbeat_errors': 0,
            'tx_packets': 2494735,
            'tx_window_errors': 0},
 'stats': {'mulicast': 0,
           'rx_bytes': 1090835789,
           'rx_compressed': 0,
           'rx_crc_errors': 0,
           'rx_dropped': 16,
           'rx_errors': 0,
           'rx_fifo_errors': 0,
           'rx_frame_errors': 0,
           'rx_length_errors': 0,
           'rx_missed_errors': 0,
           'rx_over_errors': 0,
           'rx_packets': 4057593,
           'tx_aborted_errors': 0,
           'tx_bytes': 277249054,
           'tx_carrier_errors': 0,
           'tx_compressed': 0,
           'tx_dropped': 0,
           'tx_errors': 0,
           'tx_fifo_errors': 0,
           'tx_heartbeat_errors': 0,
           'tx_packets': 2494735,
           'tx_window_errors': 0},
 'tx_queues': 4,
 'txqlen': 1000}
``` 

