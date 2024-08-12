# ForecastingProject
Estimating and forecasting service metrics from device measurements. Project work at KTH in Stockholm - completed in December 2022.

## Project 1: Estimating Service Metrics from Device Measurements
In this project, different regression models were trained in order to predict service-level metrics from infrastructure measurements. The service is either a video-on-demand system (VoD) or a key-value store (KV) with respective service-level metrics video frame rate and response time experienced by the client. Moreover, for each service a load generator was built that controls the load on the server [[1]](#1). In particular, for the VoD application it controls the number of active VoD sessions and for the KV store it manages the KV operations issued per second. Moreover, there are two load patterns, namely the periodic-load pattern as well as the flashcrowd-load pattern; for more details see [[1]](#1). Here, the flashcrowd-load pattern is the one of interest.

The project is divided into five tasks with each of those having different emphasis’. However, the overall objective is to apply several machine learning models in conjunction with various pre-processing techniques and evaluate their performances. 

[[Project Report]](https://github.com/ShriyaBhatija/ForecastingProject/blob/main/Project%201/Project_1.pdf)

## Project 2: Forecasting Service Metrics
This project aims to forecast service metrics of infrastructure measurements, particularly of a Key-Value (KV) store and of a Video-on-Demand (VoD) service based on traces collected from a KTH testbed [1] (as used previously in project 1) and the FedCSIS 2020 challenge dataset. The FedCSIS trace is a publically available dataset that is provided by the analytics company EMCA Software. It contains around 2000 samples collected over a period of roughly three months. Each sample is aggregated from measurements over one hour, hence there are 24 samples per day. The data is gathered from several hosts and for this project we will use the statistics collected from one of the hosts. In regards to the KTH testbed, the service metrics of interest are ReadsAvg for the KV service and DispFrames for the VoD service. We concatenated the datasets JNSM KV flashcrowd 1 with JNSM KV flashcrowd 2 and JNSM VoD flashcrowd 1 with JNSM VoD flashcrowd 2. Hence, we now have a larger trace for each service and will use them for the means of forecasting service metrics.

The project is divided into four tasks with each of those having different emphasis’. However, the overall objective is to apply machine learning models for forecasting and evaluate their performances.

[[Project Report]](https://github.com/ShriyaBhatija/ForecastingProject/blob/main/Project%202/Project_2.pdf)


## References
<a id="1">[1]</a> 
Rolf Stadler, Rafael Pasquini, and Viktoria Fodor. 
Learning from network device statistics. 
Journal of Network and Systems Management, 25:1–27, 10 2017.



