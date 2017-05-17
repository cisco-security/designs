################################################################################
#                                                                                                                                                            #
# Copyright (c) 2017 Cisco Systems                                                                                                      #
# All Rights Reserved.                                                                                                                            #
#                                                                                                                                                            #
#    Licensed under the Apache License, Version 2.0 (the "License"); you may                                       #
#    not use this file except in compliance with the License. You may obtain                                        #
#    a copy of the License at                                                                                                                   #
#                                                                                                                                                            #
#         http://www.apache.org/licenses/LICENSE-2.0                                                                          #
#                                                                                                                                                            #
#    Unless required by applicable law or agreed to in writing, software                                                #
#    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT                                    #
#    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the                            #
#    License for the specific language governing permissions and limitations                                      #
#    under the License.                                                                                                                           #
#                                                                                                                                                            #
################################################################################

Cisco ASA cluster & FTD cluster using FPR4150s with Nexus5548 switches in vPC
===================================================

The configuration files posted showcase how to use FPR4100 appliances and Nexus5000 switches,
and build a spanned mode setup with ASA cluster and FTD cluster.  Clustering feature scales devices
up to 16-nodes, all managed as one on the master unit, and extends connection state tracking.
To help with review of this setup, Overview videos were created on YouTube.

Here are the configurations included:

Two Nexus5000 switches in vPC (virtual port-channels match up to spanned port-channels on ASA/FTD)
-----------------------------------------------------------------------------------
nexus5548-sw1.cfg
nexus5548-sw2.cfg

Two Firepower4100 appliances in ASA cluster - Multiple contexts, all in routed firewall mode
-------------------------------------------------------------------------
fpr4150-asa-master.cfg
fpr4150-asa-slave.cfg

Cisco Firepower NGFW - ASA App Playlist:
https://www.youtube.com/playlist?list=PL_VvDNvGnyZ3JUoG8D4NBY-cTbiISb8Cc

FPR4100 ASA App Cluster: (1) Overview: https://youtu.be/7XODTR3vP8E

FPR4100 ASA App Cluster: (2) Data and CCL Resiliency: https://youtu.be/V6w6dPY9nO8

FPR4100 ASA App Cluster: (3) ASA Unit Resiliency: https://youtu.be/OvbS_qyw1w8


Two Firepower4100 appliances in FTD cluster - BVIs in transparent firewall mode 
----------------------------------------------------------------
FTD devices are managed from FMC, and those configurations are shown in the GUI.

Cisco Firepower NGFW – FTD App Playlist:
https://www.youtube.com/playlist?list=PL_VvDNvGnyZ14_Ln06R_v6m3FrzCAXad3

FPR4100 FTD App Cluster: (1) Overview: https://youtu.be/lANuLtEIS-Q

FPR4100 FTD App Cluster: (2) Data Link Resiliency: https://youtu.be/YhPhhZ5MV1Q

FPR4100 FTD App Cluster: (3) Control Link Resiliency: https://youtu.be/nhCe3TS2qds

FPR4100 FTD App Cluster: (4) Unit Loss Resiliency: https://youtu.be/xdmWoXA4wyc
                                 
FPR4100 FTD App Cluster: (5) Switch Loss Resiliency: https://youtu.be/BE0qgksJbQM





