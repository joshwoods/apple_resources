

- Kernel
- Kernel Data Types
-  tcpstat 

# tcpstat

macOS 12.0+

``` source
struct tcpstat {
    ...
};
```

## Topics

### Instance Properties

tcps_accepts

tcps_avoid_rxmt

tcps_badrst

tcps_badsyn

tcps_bg_rcvtotal

tcps_cachedrtt

tcps_cachedrttvar

tcps_cachedssthresh

tcps_closed

tcps_connattempt

tcps_conndrops

tcps_connects

tcps_delack

tcps_delay_recovery

tcps_detect_reordering

tcps_drop_after_sleep

tcps_drops

tcps_dsack_ackloss

tcps_dsack_badrexmt

tcps_dsack_disable

tcps_dsack_recvd

tcps_dsack_recvd_old

tcps_dsack_sent

tcps_early_rexmt

tcps_ecn_ace_recv_ce

tcps_ecn_ace_syn_ce

tcps_ecn_ace_syn_ect0

tcps_ecn_ace_syn_ect1

tcps_ecn_ace_syn_not_ect

tcps_ecn_client_setup

tcps_ecn_client_success

tcps_ecn_conn_nopl_ce

tcps_ecn_conn_pl_ce

tcps_ecn_conn_plnoce

tcps_ecn_conn_recv_ce

tcps_ecn_conn_recv_ece

tcps_ecn_fallback_ce

tcps_ecn_fallback_droprst

tcps_ecn_fallback_droprxmt

tcps_ecn_fallback_reorder

tcps_ecn_fallback_synloss

tcps_ecn_fallback_synrst

tcps_ecn_lost_syn

tcps_ecn_lost_synack

tcps_ecn_not_supported

tcps_ecn_recv_ce

tcps_ecn_recv_ece

tcps_ecn_sent_ece

tcps_ecn_server_setup

tcps_ecn_server_success

tcps_estab_fallback

tcps_fcholdpacket

tcps_fin_timeout_drops

tcps_hc_added

tcps_hc_bucketoverflow

tcps_invalid_joins

tcps_invalid_mpcap

tcps_invalid_opt

tcps_join_fallback

tcps_join_rxmts

tcps_ka_offload_drops

tcps_keepdrops

tcps_keepprobe

tcps_keeptimeo

tcps_limited_txt

tcps_listendrop

tcps_minmssdrops

tcps_mp_badcsum

tcps_mp_num_probes

tcps_mp_oodata

tcps_mp_outofwin

tcps_mp_rcvbytes

tcps_mp_rcvtotal

tcps_mp_reducedwin

tcps_mp_sel_peer

tcps_mp_sel_rto

tcps_mp_sel_rtt

tcps_mp_sel_symtomsd

tcps_mp_sndbytes

tcps_mp_sndpacks

tcps_mp_switches

tcps_mp_verdowngrade

tcps_mpcap_fallback

tcps_mptcp_aggregate_all_bytes

tcps_mptcp_aggregate_attempt

tcps_mptcp_aggregate_cell_bytes

tcps_mptcp_aggregate_success

tcps_mptcp_back_to_wifi

tcps_mptcp_cell_proxy

tcps_mptcp_fp_aggregate_attempt

tcps_mptcp_fp_aggregate_success

tcps_mptcp_fp_handover_attempt

tcps_mptcp_fp_handover_success_cell

tcps_mptcp_fp_handover_success_wifi

tcps_mptcp_fp_heuristic_fallback

tcps_mptcp_fp_interactive_attempt

tcps_mptcp_fp_interactive_success

tcps_mptcp_handover_all_bytes

tcps_mptcp_handover_attempt

tcps_mptcp_handover_cell_bytes

tcps_mptcp_handover_cell_from_wifi

tcps_mptcp_handover_success_cell

tcps_mptcp_handover_success_wifi

tcps_mptcp_handover_wifi_from_cell

tcps_mptcp_heuristic_fallback

tcps_mptcp_interactive_all_bytes

tcps_mptcp_interactive_attempt

tcps_mptcp_interactive_cell_bytes

tcps_mptcp_interactive_cell_from_wifi

tcps_mptcp_interactive_success

tcps_mptcp_rcvduppack

tcps_mptcp_rcvmemdrop

tcps_mptcp_rcvpackafterwin

tcps_mptcp_triggered_cell

tcps_mptcp_wifi_proxy

tcps_mss_to_default

tcps_mss_to_low

tcps_mss_to_medium

tcps_mturesent

tcps_nostretchack

tcps_pawsdrop

tcps_pcbcachemiss

tcps_persistdrop

tcps_persisttimeo

tcps_pmtudbh_reverted

tcps_predack

tcps_preddat

tcps_probe_if

tcps_probe_if_conflict

tcps_pto

tcps_pto_in_recovery

tcps_rack_recovery_episode

tcps_rack_reordering_timeout_recovery_episode

tcps_rack_rexmits

tcps_rcv6_swcsum

tcps_rcv6_swcsum_bytes

tcps_rcv_swcsum

tcps_rcv_swcsum_bytes

tcps_rcvackbyte

tcps_rcvackpack

tcps_rcvacktoomuch

tcps_rcvafterclose

tcps_rcvbadoff

tcps_rcvbadsum

tcps_rcvbyte

tcps_rcvbyteafterwin

tcps_rcvdupack

tcps_rcvdupbyte

tcps_rcvduppack

tcps_rcvmemdrop

tcps_rcvoobyte

tcps_rcvoopack

tcps_rcvpack

tcps_rcvpackafterwin

tcps_rcvpartdupbyte

tcps_rcvpartduppack

tcps_rcvshort

tcps_rcvtotal

tcps_rcvwinprobe

tcps_rcvwinupd

tcps_recovered_pkts

tcps_reordered_pkts

tcps_rescue_rxmt

tcps_rexmttimeo

tcps_rstchallenge

tcps_rto_after_pto

tcps_rttupdated

tcps_rxtfindrop

tcps_sack_ackadv

tcps_sack_rcv_blocks

tcps_sack_recovery_episode

tcps_sack_rexmit_bytes

tcps_sack_rexmits

tcps_sack_sboverflow

tcps_sack_send_blocks

tcps_sc_aborted

tcps_sc_added

tcps_sc_badack

tcps_sc_bucketoverflow

tcps_sc_cacheoverflow

tcps_sc_completed

tcps_sc_dropped

tcps_sc_dupsyn

tcps_sc_recvcookie

tcps_sc_reset

tcps_sc_retransmitted

tcps_sc_sendcookie

tcps_sc_stale

tcps_sc_unreach

tcps_sc_zonefail

tcps_segstimed

tcps_snd6_swcsum

tcps_snd6_swcsum_bytes

tcps_snd_swcsum

tcps_snd_swcsum_bytes

tcps_sndacks

tcps_sndbyte

tcps_sndctrl

tcps_sndpack

tcps_sndprobe

tcps_sndrexmitbad

tcps_sndrexmitbyte

tcps_sndrexmitpack

tcps_sndtotal

tcps_sndurg

tcps_sndwinup

tcps_synchallenge

tcps_tailloss_rto

tcps_tfo_blackhole

tcps_tfo_cookie_invalid

tcps_tfo_cookie_rcv

tcps_tfo_cookie_req

tcps_tfo_cookie_req_rcv

tcps_tfo_cookie_sent

tcps_tfo_cookie_wrong

tcps_tfo_heuristics_disable

tcps_tfo_no_cookie_rcv

tcps_tfo_sndblackhole

tcps_tfo_syn_data_acked

tcps_tfo_syn_data_rcv

tcps_tfo_syn_data_sent

tcps_tfo_syn_loss

tcps_timeoutdrop

tcps_timer_drift_gt_1000_ms

tcps_timer_drift_le_1000_ms

tcps_timer_drift_le_100_ms

tcps_timer_drift_le_10_ms

tcps_timer_drift_le_1_ms

tcps_timer_drift_le_200_ms

tcps_timer_drift_le_20_ms

tcps_timer_drift_le_500_ms

tcps_timer_drift_le_50_ms

tcps_tlp_recoverlastpkt

tcps_tlp_recovery

tcps_unnecessary_rxmt

tcps_unused_1

tcps_unused_2

tcps_unused_3

tcps_usedrtt

tcps_usedrttvar

tcps_usedssthresh

