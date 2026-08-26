SAS Viya Forecasting Pipelines
=============================

## Overview
SAS Visual Forecasting, the new-generation forecasting product from SAS, includes a web-based user interface for creating and running projects that generate forecasts from historical data. It is designed to use the highly parallel and distributed architecture of SAS® Viya®, a cloud-enabled, in-memory analytics engine that is powered by SAS® Cloud Analytic Services (CAS), to effectively model and forecast time series on a large scale. SAS Visual Forecasting includes several built-in modeling strategies, which serve as ready-to-use models for generating forecasts. It also supports custom modeling nodes, where you can write and import your own code-based modeling strategies. Similar to the ready-to-use models, these custom modeling nodes can also be shared with other projects and forecasters. Forecasters can use SAS Visual Forecasting to create projects by using visual flow diagrams (called pipelines), running multiple built-in or custom models on the same data, and choosing a champion model based on the results. 

This repository provides custom pipeline and modeling nodes in SAS Visual Forecasting.

## Custom modeling nodes:
| File name  | VF version | Description |
| ------------- | ------------- | ------------- |
| Gradient Boosting Model.zip  | Viya 4  | Example of a custom code node using Gradient Boosting for time series forecasting. Details are in the SGF Paper SAS3258-2019, **Writing a Gradient Boosting Model Node for SAS® Visual Forecasting**, downloadable at [click here](https://www.sas.com/content/dam/SAS/support/en/sas-global-forum-proceedings/2019/3258-2019.pdf).|
| VF_RNN_ATSM_NODE.zip  | Viya 4  | A SAS® Visual Forcasting custom node for recurrent neural network(RNN) forecasting. The node uses the ATSM package and the RNNSPEC in the TSM package of PROC TSMODEL. The RNN options are found at https://go.documentation.sas.com/doc/en/pgmsascdc/v_045/castsp/castsp_tsm_sect129.htm and some implemented RNN details are in https://go.documentation.sas.com/doc/en/pgmsascdc/v_045/castsp/castsp_tnf_sect037.htm |   
| Custom_Seasonal_Model_INEVENT_INEVENTBY.zip  | Viya 4  | Custom Seasonal Modeling Node with support for node-level event definitions (INEVENT) and BY-group-aware event mappings (INEVENTBY). See the [EVENTBY Documentation](https://go.documentation.sas.com/doc/en/pgmsascdc/v_075/hpfug/hpfug_hpfdiag_details33.htm#hpfug.hpfdiag.diagdetaileventby). |

