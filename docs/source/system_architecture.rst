SYSTEM ARCHITECTURE 
===================

General overview 
----------------

Seasonal outlooks of crop and water supply failures provided by
InfoSequia rest on the application of a machine learning algorithm that
is trained with a suite of EO-based drought and climate-teleconection
indices which act as potential predictors. These indices, or predictors,
which are computed at different timescales module aim to provide the
most reliable and accurate picture of the drought status of a particular
geographical region including its magnitude, severity, spatial extent
and persistence. InfoSequia indices embrace the most widely used drought
definitions, i.e. meteorological, vegetative or agronomical, and
hydrological and hydrogeological.

InfoSequia is composed of three main modules:

1) The IS-MONITOR module, which includes a set of algorithms that
   compute up-to-date drought indices based on Earth Observation (EO)
   and climate data stored in cloud platforms.

2) The IS-4CAST, which uses a machine-learning technique for producing
   region-specific alerts based on seasonal-scale forecasts of drought
   probability.

3) The IS-VIEWER, which includes the front-end solutions and app
   specifically design for sharing and viewing data. Outcomes of the
   IS-MONITOR and IS-4CAST modules are fed into drought bulletins or a
   web-mapping interface, or into existing Platform-as-a-Service (PaaS)
   solutions.

InfoSequia relies in several software and analytical tools that are
involved either for coding development and testing, cloud computing and
hosting platforms, operational running of scripts, and storing, sharing
and publication of outcomes. In addition, the system relies on external
repositories that provide the raw EO and climate data needed for
up-to-date drought and teleconnection indices.

|Diagram Description automatically generated|

Figure . System architecture of InfoSequia (functional block diagram)

.. |Diagram Description automatically generated| image:: ./media/image4.png
   :width: 5.73913in
   :height: 3.22806in