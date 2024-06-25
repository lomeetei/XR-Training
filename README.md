# XR-Training
{
    "plugins": "xr_sim_launch.py,/auto/firex/STAGING_21986/firex/venv/lib/python3.9/site-packages/firex_cisco/testy/bin/testy_launch.py,/auto/firex/STAGING_21986/firex/venv/lib/python3.9/site-packages/firex_cisco/testy/plugins/testy_common_plugin.py",
    "decomm_tb_after_test": true,
    "data": {
        "ws": "/ws/pulakra-bgl/xr",
        "plat": "8000",
        "framework": "cafy2",
        "topo_file": "/ws/pulakra-bgl/xr/test/ap/training/F2_Spitfire_Template.yaml",
        "testbed_logs_dir": "/auto/firex-logs-bgl/pulakra/FireX-pulakra-240625-035946-38901/testbed_logs/BringupTestbed-9c93600d-d8dd-4f79-a068-15bcadd58b27",
        "xunit_results_filepath": "/auto/firex-logs-bgl/pulakra/FireX-pulakra-240625-035946-38901/tests_logs/training_ap_8000_34996E7B/xunit_results.xml",
        "logstash_container_id": null,
        "replace_script_name": "training_ap.py --test-input-file=/ws/pulakra-bgl/xr/test/ap/training/training_ap_input_file.json",
        "image_name": null,
        "images": null,
        "spirent_image_basepath": "/auto/vxr/images/spirent/",
        "ixia_image_basepath": "/auto/vxr/images/ixia/",
        "sim_rel": null,
        "sim_host": "xr-cloud-213",
        "use_aws": false,
        "logstash_ip_address": null,
        "logstash_port": null,
        "moonshine_img": null,
        "moonshine_img_v2": null,
        "testbed": "/auto/firex-logs-bgl/pulakra/FireX-pulakra-240625-035946-38901/service_data/BootVxSim/task_data/f9e09c34-cdeb-4ec9-a500-61ed509d0841/cafy2_tb_file.json",
        "testbed_path": null,
        "topology": {
            "devices": {
                "R1": {
                    "xr_port_redir": [
                        22,
                        830
                    ],
                    "platform": "spitfire_f",
                    "xr_config": "ssh server vrf default\nssh server netconf vrf default\nnetconf-yang agent ssh\n",
                    "data_ports": [
                        "FourHundredGigE0/0/0/0",
                        "FourHundredGigE0/0/0/1",
                        "FourHundredGigE0/0/0/2",
                        "FourHundredGigE0/0/0/3",
                        "FourHundredGigE0/0/0/4",
                        "FourHundredGigE0/0/0/5",
                        "FourHundredGigE0/0/0/6",
                        "FourHundredGigE0/0/0/7"
                    ],
                    "image": "/ws/pulakra-bgl/xr/img-8000/8000-x64.iso",
                    "sim_host": "xr-cloud-213"
                },
                "R2": {
                    "xr_port_redir": [
                        22,
                        830
                    ],
                    "platform": "spitfire_f",
                    "xr_config": "ssh server vrf default\nssh server netconf vrf default\nnetconf-yang agent ssh\n",
                    "data_ports": [
                        "FourHundredGigE0/0/0/0",
                        "FourHundredGigE0/0/0/1",
                        "FourHundredGigE0/0/0/2",
                        "FourHundredGigE0/0/0/3",
                        "FourHundredGigE0/0/0/4",
                        "FourHundredGigE0/0/0/5",
                        "FourHundredGigE0/0/0/6",
                        "FourHundredGigE0/0/0/7"
                    ],
                    "image": "/ws/pulakra-bgl/xr/img-8000/8000-x64.iso",
                    "sim_host": "xr-cloud-213"
                }
            },
            "connections": {
                "hubs": {
                    "R1_R2_1": [
                        "R1.FourHundredGigE0/0/0/0",
                        "R2.FourHundredGigE0/0/0/0"
                    ],
                    "R1_R2_2": [
                        "R1.FourHundredGigE0/0/0/1",
                        "R2.FourHundredGigE0/0/0/1"
                    ],
                    "R1_R2_3": [
                        "R1.FourHundredGigE0/0/0/2",
                        "R2.FourHundredGigE0/0/0/2"
                    ],
                    "R1_R2_4": [
                        "R1.FourHundredGigE0/0/0/3",
                        "R2.FourHundredGigE0/0/0/3"
                    ],
                    "R1_R2_5": [
                        "R1.FourHundredGigE0/0/0/4",
                        "R2.FourHundredGigE0/0/0/4"
                    ],
                    "R1_R2_6": [
                        "R1.FourHundredGigE0/0/0/5",
                        "R2.FourHundredGigE0/0/0/5"
                    ],
                    "R1_R2_7": [
                        "R1.FourHundredGigE0/0/0/6",
                        "R2.FourHundredGigE0/0/0/6"
                    ],
                    "R1_R2_8": [
                        "R1.FourHundredGigE0/0/0/7",
                        "R2.FourHundredGigE0/0/0/7"
                    ]
                }
            },
            "simulation": {
                "sim_rel": "/auto/vxr/vxr2_user/vxr2_npsuite_1.113.1",
                "sim_dir": "/nobackup/pulakra/FireX-pulakra-240625-035946-38901-6664",
                "sim_host": "xr-cloud-213",
                "sim_host_username": "pulakra"
            }
        },
        "slurm_cluster_head": "xr-cloud-m201",
        "slurm_jobid": "6664",
        "cflow_vxr_server": "xr-cloud-213",
        "topo_path": "/ws/pulakra-bgl/xr/test/ap/training/F2_Spitfire_Template.yaml",
        "sim_working_dir": "/auto/firex-logs-bgl/pulakra/FireX-pulakra-240625-035946-38901/service_data/BootVxSim/task_data/f9e09c34-cdeb-4ec9-a500-61ed509d0841",
        "tb_data": {
            "name": "generated-vxsim",
            "nodes": [
                {
                    "name": "R1",
                    "alias": "R1",
                    "type": "router",
                    "platform": "SPITFIRE_F",
                    "os": "thinxr",
                    "credential": "R1cred",
                    "access_info": [
                        {
                            "name": "console",
                            "interface": "console",
                            "address_info": [
                                {
                                    "name": "a",
                                    "address": "10.104.60.193",
                                    "port": 26217
                                }
                            ]
                        },
                        {
                            "name": "vty",
                            "interface": "vty",
                            "address_info": [
                                {
                                    "name": "ssh",
                                    "address": "10.104.60.193",
                                    "port": 12285
                                }
                            ]
                        }
                    ],
                    "handles": [
                        {
                            "via": "console",
                            "name": "console",
                            "credential": "R1cred",
                            "connection": "ha",
                            "global_delay_factor": 5
                        },
                        {
                            "via": "vty.ssh",
                            "name": "ssh",
                            "credential": "R1cred",
                            "connection": "ssh",
                            "global_delay_factor": 5,
                            "default": true
                        }
                    ],
                    "interfaces": [
                        {
                            "interface": "FourHundredGigE0/0/0/0",
                            "link": "R1_R2_1",
                            "alias": "R1_R2_1"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/1",
                            "link": "R1_R2_2",
                            "alias": "R1_R2_2"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/2",
                            "link": "R1_R2_3",
                            "alias": "R1_R2_3"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/3",
                            "link": "R1_R2_4",
                            "alias": "R1_R2_4"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/4",
                            "link": "R1_R2_5",
                            "alias": "R1_R2_5"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/5",
                            "link": "R1_R2_6",
                            "alias": "R1_R2_6"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/6",
                            "link": "R1_R2_7",
                            "alias": "R1_R2_7"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/7",
                            "link": "R1_R2_8",
                            "alias": "R1_R2_8"
                        }
                    ]
                },
                {
                    "name": "R2",
                    "alias": "R2",
                    "type": "router",
                    "platform": "SPITFIRE_F",
                    "os": "thinxr",
                    "credential": "R2cred",
                    "access_info": [
                        {
                            "name": "console",
                            "interface": "console",
                            "address_info": [
                                {
                                    "name": "a",
                                    "address": "10.104.60.193",
                                    "port": 17813
                                }
                            ]
                        },
                        {
                            "name": "vty",
                            "interface": "vty",
                            "address_info": [
                                {
                                    "name": "ssh",
                                    "address": "10.104.60.193",
                                    "port": 19613
                                }
                            ]
                        }
                    ],
                    "handles": [
                        {
                            "via": "console",
                            "name": "console",
                            "credential": "R2cred",
                            "connection": "ha",
                            "global_delay_factor": 5
                        },
                        {
                            "via": "vty.ssh",
                            "name": "ssh",
                            "credential": "R2cred",
                            "connection": "ssh",
                            "global_delay_factor": 5,
                            "default": true
                        }
                    ],
                    "interfaces": [
                        {
                            "interface": "FourHundredGigE0/0/0/0",
                            "link": "R1_R2_1",
                            "alias": "R1_R2_1"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/1",
                            "link": "R1_R2_2",
                            "alias": "R1_R2_2"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/2",
                            "link": "R1_R2_3",
                            "alias": "R1_R2_3"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/3",
                            "link": "R1_R2_4",
                            "alias": "R1_R2_4"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/4",
                            "link": "R1_R2_5",
                            "alias": "R1_R2_5"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/5",
                            "link": "R1_R2_6",
                            "alias": "R1_R2_6"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/6",
                            "link": "R1_R2_7",
                            "alias": "R1_R2_7"
                        },
                        {
                            "interface": "FourHundredGigE0/0/0/7",
                            "link": "R1_R2_8",
                            "alias": "R1_R2_8"
                        }
                    ]
                }
            ],
            "credentials": [
                {
                    "name": "R1cred",
                    "username": "cisco",
                    "password": "cisco123"
                },
                {
                    "name": "R2cred",
                    "username": "cisco",
                    "password": "cisco123"
                }
            ],
            "simulation": {
                "sim_rel": "/auto/vxr/vxr2_user/vxr2_npsuite_1.113.1",
                "sim_dir": "/nobackup/pulakra/FireX-pulakra-240625-035946-38901-6664",
                "sim_host": "xr-cloud-213",
                "sim_host_username": "pulakra",
                "sim_host_password": ""
            }
        },
        "moonshine_host": null,
        "testbed_launched": true,
        "router_data_collector": false
    }
}
