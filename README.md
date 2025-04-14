# Daily Papers
The project automatically fetches the latest papers from arXiv based on keywords.

The subheadings in the README file represent the search keywords.

Only the most recent articles for each keyword are retained, up to a maximum of 100 papers.

You can click the 'Watch' button to receive daily email notifications.

Last update: 2025-04-14

## Time Series
| **Title** | **Date** | **Abstract** | **Comment** |
| --- | --- | --- | --- |
| **[Semantically Encoding Activity Labels for Context-Aware Human Activity Recognition](http://arxiv.org/abs/2504.07916v1)** | 2025-04-10 | <details><summary>Show</summary><p>Prior work has primarily formulated CA-HAR as a multi-label classification problem, where model inputs are time-series sensor data and target labels are binary encodings representing whether a given activity or context occurs. These CA-HAR methods either predicted each label independently or manually imposed relationships using graphs. However, both strategies often neglect an essential aspect: activity labels have rich semantic relationships. For instance, walking, jogging, and running activities share similar movement patterns but differ in pace and intensity, indicating that they are semantically related. Consequently, prior CA-HAR methods often struggled to accurately capture these inherent and nuanced relationships, particularly on datasets with noisy labels typically used for CA-HAR or situations where the ideal sensor type is unavailable (e.g., recognizing speech without audio sensors). To address this limitation, we propose SEAL, which leverage LMs to encode CA-HAR activity labels to capture semantic relationships. LMs generate vector embeddings that preserve rich semantic information from natural language. Our SEAL approach encodes input-time series sensor data from smart devices and their associated activity and context labels (text) as vector embeddings. During training, SEAL aligns the sensor data representations with their corresponding activity/context label embeddings in a shared embedding space. At inference time, SEAL performs a similarity search, returning the CA-HAR label with the embedding representation closest to the input data. Although LMs have been widely explored in other domains, surprisingly, their potential in CA-HAR has been underexplored, making our approach a novel contribution to the field. Our research opens up new possibilities for integrating more advanced LMs into CA-HAR tasks.</p></details> | Percom 2025 |
| **[ms-Mamba: Multi-scale Mamba for Time-Series Forecasting](http://arxiv.org/abs/2504.07654v1)** | 2025-04-10 | <details><summary>Show</summary><p>The problem of Time-series Forecasting is generally addressed by recurrent, Transformer-based and the recently proposed Mamba-based architectures. However, existing architectures generally process their input at a single temporal scale, which may be sub-optimal for many tasks where information changes over multiple time scales. In this paper, we introduce a novel architecture called Multi-scale Mamba (ms-Mamba) to address this gap. ms-Mamba incorporates multiple temporal scales by using multiple Mamba blocks with different sampling rates ($\Delta$s). Our experiments on many benchmarks demonstrate that ms-Mamba outperforms state-of-the-art approaches, including the recently proposed Transformer-based and Mamba-based models.</p></details> |  |
| **[Diffusion Transformers for Tabular Data Time Series Generation](http://arxiv.org/abs/2504.07566v1)** | 2025-04-10 | <details><summary>Show</summary><p>Tabular data generation has recently attracted a growing interest due to its different application scenarios. However, generating time series of tabular data, where each element of the series depends on the others, remains a largely unexplored domain. This gap is probably due to the difficulty of jointly solving different problems, the main of which are the heterogeneity of tabular data (a problem common to non-time-dependent approaches) and the variable length of a time series. In this paper, we propose a Diffusion Transformers (DiTs) based approach for tabular data series generation. Inspired by the recent success of DiTs in image and video generation, we extend this framework to deal with heterogeneous data and variable-length sequences. Using extensive experiments on six datasets, we show that the proposed approach outperforms previous work by a large margin.</p></details> | <details><summary>26 pa...</summary><p>26 pages, 19 figures, 13 tables</p></details> |
| **[Event Signal Filtering via Probability Flux Estimation](http://arxiv.org/abs/2504.07503v1)** | 2025-04-10 | <details><summary>Show</summary><p>Events offer a novel paradigm for capturing scene dynamics via asynchronous sensing, but their inherent randomness often leads to degraded signal quality. Event signal filtering is thus essential for enhancing fidelity by reducing this internal randomness and ensuring consistent outputs across diverse acquisition conditions. Unlike traditional time series that rely on fixed temporal sampling to capture steady-state behaviors, events encode transient dynamics through polarity and event intervals, making signal modeling significantly more complex. To address this, the theoretical foundation of event generation is revisited through the lens of diffusion processes. The state and process information within events is modeled as continuous probability flux at threshold boundaries of the underlying irradiance diffusion. Building on this insight, a generative, online filtering framework called Event Density Flow Filter (EDFilter) is introduced. EDFilter estimates event correlation by reconstructing the continuous probability flux from discrete events using nonparametric kernel smoothing, and then resamples filtered events from this flux. To optimize fidelity over time, spatial and temporal kernels are employed in a time-varying optimization framework. A fast recursive solver with O(1) complexity is proposed, leveraging state-space models and lookup tables for efficient likelihood computation. Furthermore, a new real-world benchmark Rotary Event Dataset (RED) is released, offering microsecond-level ground truth irradiance for full-reference event filtering evaluation. Extensive experiments validate EDFilter's performance across tasks like event filtering, super-resolution, and direct event-based blob tracking. Significant gains in downstream applications such as SLAM and video reconstruction underscore its robustness and effectiveness.</p></details> |  |
| **[Estimation of High-Dimensional Markov-Switching VAR Models with an Approximate EM Algorithm](http://arxiv.org/abs/2210.07456v2)** | 2025-04-10 | <details><summary>Show</summary><p>Regime shifts in high-dimensional time series arise naturally in many applications, from neuroimaging to finance. This problem has received considerable attention in low-dimensional settings, with both Bayesian and frequentist methods used extensively for parameter estimation. The EM algorithm is a particularly popular strategy for parameter estimation in low-dimensional settings, although the statistical properties of the resulting estimates have not been well understood. Furthermore, its extension to high-dimensional time series has proved challenging. To overcome these challenges, in this paper we propose an approximate EM algorithm for Markov-switching VAR models that leads to efficient computation and also facilitates the investigation of asymptotic properties of the resulting parameter estimates. We establish the consistency of the proposed EM algorithm in high dimensions and investigate its performance via simulation studies. We also demonstrate the algorithm by analyzing a brain electroencephalography (EEG) dataset recorded on a patient experiencing epileptic seizure.</p></details> |  |
| **[AMAD: AutoMasked Attention for Unsupervised Multivariate Time Series Anomaly Detection](http://arxiv.org/abs/2504.06643v2)** | 2025-04-10 | <details><summary>Show</summary><p>Unsupervised multivariate time series anomaly detection (UMTSAD) plays a critical role in various domains, including finance, networks, and sensor systems. In recent years, due to the outstanding performance of deep learning in general sequential tasks, many models have been specialized for deep UMTSAD tasks and have achieved impressive results, particularly those based on the Transformer and self-attention mechanisms. However, the sequence anomaly association assumptions underlying these models are often limited to specific predefined patterns and scenarios, such as concentrated or peak anomaly patterns. These limitations hinder their ability to generalize to diverse anomaly situations, especially where the lack of labels poses significant challenges. To address these issues, we propose AMAD, which integrates \textbf{A}uto\textbf{M}asked Attention for UMTS\textbf{AD} scenarios. AMAD introduces a novel structure based on the AutoMask mechanism and an attention mixup module, forming a simple yet generalized anomaly association representation framework. This framework is further enhanced by a Max-Min training strategy and a Local-Global contrastive learning approach. By combining multi-scale feature extraction with automatic relative association modeling, AMAD provides a robust and adaptable solution to UMTSAD challenges. Extensive experimental results demonstrate that the proposed model achieving competitive performance results compared to SOTA benchmarks across a variety of datasets.</p></details> | fix img issues |
| **[ClimateBench-M: A Multi-Modal Climate Data Benchmark with a Simple Generative Method](http://arxiv.org/abs/2504.07394v1)** | 2025-04-10 | <details><summary>Show</summary><p>Climate science studies the structure and dynamics of Earth's climate system and seeks to understand how climate changes over time, where the data is usually stored in the format of time series, recording the climate features, geolocation, time attributes, etc. Recently, much research attention has been paid to the climate benchmarks. In addition to the most common task of weather forecasting, several pioneering benchmark works are proposed for extending the modality, such as domain-specific applications like tropical cyclone intensity prediction and flash flood damage estimation, or climate statement and confidence level in the format of natural language. To further motivate the artificial general intelligence development for climate science, in this paper, we first contribute a multi-modal climate benchmark, i.e., ClimateBench-M, which aligns (1) the time series climate data from ERA5, (2) extreme weather events data from NOAA, and (3) satellite image data from NASA HLS based on a unified spatial-temporal granularity. Second, under each data modality, we also propose a simple but strong generative method that could produce competitive performance in weather forecasting, thunderstorm alerts, and crop segmentation tasks in the proposed ClimateBench-M. The data and code of ClimateBench-M are publicly available at https://github.com/iDEA-iSAIL-Lab-UIUC/ClimateBench-M.</p></details> | Preprint, 29 pages |
| **[Enhancing Time Series Forecasting via Multi-Level Text Alignment with LLMs](http://arxiv.org/abs/2504.07360v1)** | 2025-04-10 | <details><summary>Show</summary><p>The adaptation of large language models (LLMs) to time series forecasting poses unique challenges, as time series data is continuous in nature, while LLMs operate on discrete tokens. Despite the success of LLMs in natural language processing (NLP) and other structured domains, aligning time series data with language-based representations while maintaining both predictive accuracy and interpretability remains a significant hurdle. Existing methods have attempted to reprogram time series data into text-based forms, but these often fall short in delivering meaningful, interpretable results. In this paper, we propose a multi-level text alignment framework for time series forecasting using LLMs that not only improves prediction accuracy but also enhances the interpretability of time series representations. Our method decomposes time series into trend, seasonal, and residual components, which are then reprogrammed into component-specific text representations. We introduce a multi-level alignment mechanism, where component-specific embeddings are aligned with pre-trained word tokens, enabling more interpretable forecasts. Experiments on multiple datasets demonstrate that our method outperforms state-of-the-art models in accuracy while providing good interpretability.</p></details> |  |
| **[A GARMA Framework for Unit-Bounded Time Series Based on the Unit-Lindley Distribution with Application to Renewable Energy Data](http://arxiv.org/abs/2504.07351v1)** | 2025-04-10 | <details><summary>Show</summary><p>The Unit-Lindley is a one-parameter family of distributions in $(0,1)$ obtained from an appropriate transformation of the Lindley distribution. In this work, we introduce a class of dynamical time series models for continuous random variables taking values in $(0,1)$ based on the Unit-Lindley distribution. The models pertaining to the proposed class are observation-driven ones for which, conditionally on a set of covariates, the random component is modeled by a Unit-Lindley distribution. The systematic component aims at modeling the conditional mean through a dynamical structure resembling the classical ARMA models. Parameter estimation in conducted using partial maximum likelihood, for which an asymptotic theory is available. Based on asymptotic results, the construction of confidence intervals, hypotheses testing, model selection, and forecasting can be carried on. A Monte Carlo simulation study is conducted to assess the finite sample performance of the proposed partial maximum likelihood approach. Finally, an application considering forecasting of the proportion of net electricity generated by conventional hydroelectric power in the United States is presented. The application show the versatility of the proposed method compared to other benchmarks models in the literature.</p></details> | <details><summary>arXiv...</summary><p>arXiv admin note: text overlap with arXiv:2502.18645</p></details> |
| **[Polyspectral Mean based Time Series Clustering of Indian Stock Market](http://arxiv.org/abs/2504.07021v1)** | 2025-04-09 | <details><summary>Show</summary><p>In this study, we employ k-means clustering algorithm of polyspectral means to analyze 49 stocks in the Indian stock market. We have used spectral and bispectral information obtained from the data, by using spectral and bispectral means with different weight functions that will give us varying insights into the temporal patterns of the stocks. In particular, the higher order polyspectral means can provide significantly more information than what we can gather from power spectra, and can also unveil nonlinear trends in a time series. Through rigorous analysis, we identify five distinctive clusters, uncovering nuanced market structures. Notably, one cluster emerges as that of a conglomerate powerhouse, featuring ADANI, BIRLA, TATA, and unexpectedly, government-owned bank SBI. Another cluster spotlights the IT sector with WIPRO and TCS, while a third combines private banks, government entities, and RELIANCE. The final cluster comprises publicly traded companies with dispersed ownership. Such clustering of stocks sheds light on intricate financial relationships within the stock market, providing valuable insights for investors and analysts navigating the dynamic landscape of the Indian stock market.</p></details> | <details><summary>Publi...</summary><p>Published in Discover Data</p></details> |
| **[An Analysis of Temporal Dropout in Earth Observation Time Series for Regression Tasks](http://arxiv.org/abs/2504.06915v1)** | 2025-04-09 | <details><summary>Show</summary><p>Missing instances in time series data impose a significant challenge to deep learning models, particularly in regression tasks. In the Earth Observation field, satellite failure or cloud occlusion frequently results in missing time-steps, introducing uncertainties in the predicted output and causing a decline in predictive performance. While many studies address missing time-steps through data augmentation to improve model robustness, the uncertainty arising at the input level is commonly overlooked. To address this gap, we introduce Monte Carlo Temporal Dropout (MC-TD), a method that explicitly accounts for input-level uncertainty by randomly dropping time-steps during inference using a predefined dropout ratio, thereby simulating the effect of missing data. To bypass the need for costly searches for the optimal dropout ratio, we extend this approach with Monte Carlo Concrete Temporal Dropout (MC-ConcTD), a method that learns the optimal dropout distribution directly. Both MC-TD and MC-ConcTD are applied during inference, leveraging Monte Carlo sampling for uncertainty quantification. Experiments on three EO time-series datasets demonstrate that MC-ConcTD improves predictive performance and uncertainty calibration compared to existing approaches. Additionally, we highlight the advantages of adaptive dropout tuning over manual selection, making uncertainty quantification more robust and accessible for EO applications.</p></details> | <details><summary>Accep...</summary><p>Accepted at Symposium on Intelligent Data Analysis (IDA 2025)</p></details> |
| **[Quantized symbolic time series approximation](http://arxiv.org/abs/2411.15209v2)** | 2025-04-09 | <details><summary>Show</summary><p>Time series are ubiquitous in numerous science and engineering domains, e.g., signal processing, bioinformatics, and astronomy. Previous work has verified the efficacy of symbolic time series representation in a variety of engineering applications due to its storage efficiency and numerosity reduction. The most recent symbolic aggregate approximation technique, ABBA, has been shown to preserve essential shape information of time series and improve downstream applications, e.g., neural network inference regarding prediction and anomaly detection in time series. Motivated by the emergence of high-performance hardware which enables efficient computation for low bit-width representations, we present a new quantization-based ABBA symbolic approximation technique, QABBA, which exhibits improved storage efficiency while retaining the original speed and accuracy of symbolic reconstruction. We prove an upper bound for the error arising from quantization and discuss how the number of bits should be chosen to balance this with other errors. An application of QABBA with large language models (LLMs) for time series regression is also presented, and its utility is investigated. By representing the symbolic chain of patterns on time series, QABBA not only avoids the training of embedding from scratch, but also achieves a new state-of-the-art on Monash regression dataset. The symbolic approximation to the time series offers a more efficient way to fine-tune LLMs on the time series regression task which contains various application domains. We further present a set of extensive experiments performed across various well-established datasets to demonstrate the advantages of the QABBA method for symbolic approximation.</p></details> |  |
| **[ODEStream: A Buffer-Free Online Learning Framework with ODE-based Adaptor for Streaming Time Series Forecasting](http://arxiv.org/abs/2411.07413v2)** | 2025-04-09 | <details><summary>Show</summary><p>Addressing the challenges of irregularity and concept drift in streaming time series is crucial for real-world predictive modelling. Previous studies in time series continual learning often propose models that require buffering long sequences, potentially restricting the responsiveness of the inference system. Moreover, these models are typically designed for regularly sampled data, an unrealistic assumption in real-world scenarios. This paper introduces ODEStream, a novel buffer-free continual learning framework that incorporates a temporal isolation layer to capture temporal dependencies within the data. Simultaneously, it leverages the capability of neural ordinary differential equations to process irregular sequences and generate a continuous data representation, enabling seamless adaptation to changing dynamics in a data streaming scenario. Our approach focuses on learning how the dynamics and distribution of historical data change over time, facilitating direct processing of streaming sequences. Evaluations on benchmark real-world datasets demonstrate that ODEStream outperforms the state-of-the-art online learning and streaming analysis baseline models, providing accurate predictions over extended periods while minimising performance degradation over time by learning how the sequence dynamics change. The implementation of ODEStream is available at: https://github.com/FtoonAbushaqra/ODEStream.git.</p></details> |  |
| **[Network inference via approximate Bayesian computation. Illustration on a stochastic multi-population neural mass model](http://arxiv.org/abs/2306.15787v3)** | 2025-04-09 | <details><summary>Show</summary><p>In this article, we propose an adapted sequential Monte Carlo approximate Bayesian computation (SMC-ABC) algorithm for network inference in coupled stochastic differential equations (SDEs) used for multivariate time series modeling. Our approach is motivated by neuroscience, specifically the challenge of estimating brain connectivity before and during epileptic seizures. To this end, we make four key contributions. First, we introduce a 6N-dimensional SDE to model the activity of N coupled neuronal populations, extending the (single-population) stochastic Jansen and Rit neural mass model used to describe human electroencephalography (EEG) rhythms, particularly epileptic activity. Second, we construct a reliable and efficient numerical splitting scheme for the model simulation. Third, we apply the proposed adapted SMC-ABC algorithm to the neural mass model and validate it on different types of simulated data. Compared to standard SMC-ABC, our approach significantly reduces computational cost by requiring fewer model simulations to reach the desired posterior region, thanks to the inclusion of binary parameters describing the presence or absence of coupling directions. Finally, we apply our method to real multi-channel EEG data, uncovering potential similarities in patients' brain activities across different epileptic seizures, as well as differences between pre-seizure and seizure periods.</p></details> | 37 pages, 22 figures |
| **[Robust Capacity Expansion Modelling for Renewable Energy Systems under Weather and Demand Uncertainty](http://arxiv.org/abs/2504.06750v1)** | 2025-04-09 | <details><summary>Show</summary><p>Future greenhouse gas neutral energy systems will be dominated by variable renewable energy technologies. However, renewable electricity generation from wind and solar technologies, as well as electricity demand, varies with the weather. This work addresses the problem of determining optimal capacities for renewable technologies in energy systems that ensure sufficient electricity supply when dealing with multi-year time-series data. An iterative algorithm is proposed that starts by optimising an arbitrary starting time-series, followed by adding additional constraints and reoptimising the modified optimisation problem until sufficient energy supply is provided for all time--series, i.e. the solution is robust to weather and demand variations. This is evaluated in a computational study on a German energy system model.The results show that the iterative algorithm finds robust solutions for an increase of 2-2.5% in total annual cost for a simplified model in gurobipy and 2.9% for a model built in the model framework ETHOS.FINE. Testing the feasibility for non robust solutions showed that supply gaps occurred in at least some of the remaining years. Based on the results of this work, ensuring feasibility within an energy system model for multiple time-series boils down to two factors: ensuring sufficient back-up capacity to overcome periods of high demand combined with low electricity generation from wind and photovoltaic, and enforcing sufficient total annual electricity generation. Our proposed open source iterative algorithm is able to ensure this. For general modelling, it is recommended to check for systematic effects of different years' time--series on energy system models especially for wind, but also for photovoltaics, include dark lull and cold period effects on generation and demand in time--series, and assess the feasibility of energy system models using different time-series.</p></details> |  |
| **[CLaSP: Learning Concepts for Time-Series Signals from Natural Language Supervision](http://arxiv.org/abs/2411.08397v2)** | 2025-04-09 | <details><summary>Show</summary><p>This paper presents CLaSP, a novel model for retrieving time-series signals using natural language queries that describe signal characteristics. The ability to search time-series signals based on descriptive queries is essential in domains such as industrial diagnostics, where data scientists often need to find signals with specific characteristics. However, existing methods rely on sketch-based inputs, predefined synonym dictionaries, or domain-specific manual designs, limiting their scalability and adaptability. CLaSP addresses these challenges by employing contrastive learning to map time-series signals to natural language descriptions. Unlike prior approaches, it eliminates the need for predefined synonym dictionaries and leverages the rich contextual knowledge of large language models (LLMs). Using the TRUCE and SUSHI datasets, which pair time-series signals with natural language descriptions, we demonstrate that CLaSP achieves high accuracy in retrieving a variety of time series patterns based on natural language queries.</p></details> |  |
| **[PyIT2FLS: A New Python Toolkit for Interval Type 2 Fuzzy Logic Systems](http://arxiv.org/abs/1909.10051v3)** | 2025-04-09 | <details><summary>Show</summary><p>Fuzzy logic is an accepted and well-developed approach for constructing verbal models. Fuzzy based methods are getting more popular, while the engineers deal with more daily life tasks. This paper presents a new Python toolkit for Interval Type 2 Fuzzy Logic Systems (IT2FLS). Developing software tools is an important issue for facilitating the practical use of theoretical results. There are limited tools for implementing IT2FLSs in Python. The developed PyIT2FLS is providing a set of tools for fast and easy modeling of fuzzy systems. This paper includes a brief description of how developed toolkit can be used. Also, three examples are given showing the usage of the developed toolkit for simulating IT2FLSs. First, a simple rule-based system is developed and it's codes are presented in the paper. The second example is the prediction of the Mackey-Glass chaotic time series using IT2FLS. In this example, the Particle Swarm Optimization (PSO) algorithm is used for determining system parameters while minimizing the mean square error. In the last example, an IT2FPID is designed and used for controlling a linear time-delay system. The code for the examples are available on toolkit's GitHub page: https://github.com/Haghrah/PyIT2FLS. The simulations and their results confirm the ability of the developed toolkit to be used in a wide range of the applications.</p></details> | <details><summary>This ...</summary><p>This work has been published in SoftwareX, Volume 30, May 2025, 102146. https://doi.org/10.1016/j.softx.2025.102146</p></details> |
| **[WaveHiTS: Wavelet-Enhanced Hierarchical Time Series Modeling for Wind Direction Nowcasting in Eastern Inner Mongolia](http://arxiv.org/abs/2504.06532v1)** | 2025-04-09 | <details><summary>Show</summary><p>Wind direction forecasting plays a crucial role in optimizing wind energy production, but faces significant challenges due to the circular nature of directional data, error accumulation in multi-step forecasting, and complex meteorological interactions. This paper presents a novel model, WaveHiTS, which integrates wavelet transform with Neural Hierarchical Interpolation for Time Series to address these challenges. Our approach decomposes wind direction into U-V components, applies wavelet transform to capture multi-scale frequency patterns, and utilizes a hierarchical structure to model temporal dependencies at multiple scales, effectively mitigating error propagation. Experiments conducted on real-world meteorological data from Inner Mongolia, China demonstrate that WaveHiTS significantly outperforms deep learning models (RNN, LSTM, GRU), transformer-based approaches (TFT, Informer, iTransformer), and hybrid models (EMD-LSTM). The proposed model achieves RMSE values of approximately 19.2{\deg}-19.4{\deg} compared to 56{\deg}-64{\deg} for deep learning recurrent models, maintaining consistent accuracy across all forecasting steps up to 60 minutes ahead. Moreover, WaveHiTS demonstrates superior robustness with vector correlation coefficients (VCC) of 0.985-0.987 and hit rates of 88.5%-90.1%, substantially outperforming baseline models. Ablation studies confirm that each component-wavelet transform, hierarchical structure, and U-V decomposition-contributes meaningfully to overall performance. These improvements in wind direction nowcasting have significant implications for enhancing wind turbine yaw control efficiency and grid integration of wind energy.</p></details> |  |
| **[TSP-OCS: A Time-Series Prediction for Optimal Camera Selection in Multi-Viewpoint Surgical Video Analysis](http://arxiv.org/abs/2504.06527v1)** | 2025-04-09 | <details><summary>Show</summary><p>Recording the open surgery process is essential for educational and medical evaluation purposes; however, traditional single-camera methods often face challenges such as occlusions caused by the surgeon's head and body, as well as limitations due to fixed camera angles, which reduce comprehensibility of the video content. This study addresses these limitations by employing a multi-viewpoint camera recording system, capturing the surgical procedure from six different angles to mitigate occlusions. We propose a fully supervised learning-based time series prediction method to choose the best shot sequences from multiple simultaneously recorded video streams, ensuring optimal viewpoints at each moment. Our time series prediction model forecasts future camera selections by extracting and fusing visual and semantic features from surgical videos using pre-trained models. These features are processed by a temporal prediction network with TimeBlocks to capture sequential dependencies. A linear embedding layer reduces dimensionality, and a Softmax classifier selects the optimal camera view based on the highest probability. In our experiments, we created five groups of open thyroidectomy videos, each with simultaneous recordings from six different angles. The results demonstrate that our method achieves competitive accuracy compared to traditional supervised methods, even when predicting over longer time horizons. Furthermore, our approach outperforms state-of-the-art time series prediction techniques on our dataset. This manuscript makes a unique contribution by presenting an innovative framework that advances surgical video analysis techniques, with significant implications for improving surgical education and patient safety.</p></details> |  |
| **[Bounds in Wasserstein Distance for Locally Stationary Functional Time Series](http://arxiv.org/abs/2504.06453v1)** | 2025-04-08 | <details><summary>Show</summary><p>Functional time series (FTS) extend traditional methodologies to accommodate data observed as functions/curves. A significant challenge in FTS consists of accurately capturing the time-dependence structure, especially with the presence of time-varying covariates. When analyzing time series with time-varying statistical properties, locally stationary time series (LSTS) provide a robust framework that allows smooth changes in mean and variance over time. This work investigates Nadaraya-Watson (NW) estimation procedure for the conditional distribution of locally stationary functional time series (LSFTS), where the covariates reside in a semi-metric space endowed with a semi-metric. Under small ball probability and mixing condition, we establish convergence rates of NW estimator for LSFTS with respect to Wasserstein distance. The finite-sample performances of the model and the estimation method are illustrated through extensive numerical experiments both on functional simulated and real data.</p></details> |  |
| **[Center-fixing of tropical cyclones using uncertainty-aware deep learning applied to high-temporal-resolution geostationary satellite imagery](http://arxiv.org/abs/2409.16507v2)** | 2025-04-08 | <details><summary>Show</summary><p>Determining the location of a tropical cyclone's (TC) surface circulation center -- "center-fixing" -- is a critical first step in the TC-forecasting process, affecting current and future estimates of track, intensity, and structure. Despite a recent increase in automated center-fixing methods, only one such method (ARCHER-2) is operational, and its best performance is achieved when using microwave or scatterometer data, which are not available at every forecast cycle. We develop a deep-learning algorithm called GeoCenter; besides a few scalars in the operational ATCF, it relies only on geostationary IR satellite imagery, which is available for all TC basins at high frequency (10 min) and low latency (< 10 min) during both day and night. GeoCenter ingests an animation (time series) of IR images, including 9 channels at lag times up to 4 hours. The animation is centered at a "first guess" location, offset from the true TC-center location by 48 km on average and sometimes > 100 km; GeoCenter is tasked with correcting this offset. On an independent testing dataset, GeoCenter achieves a mean/median/RMS (root mean square) error of 26.6/22.2/32.4 km for all systems, 24.7/20.8/30.0 km for tropical systems, and 14.6/12.5/17.3 km for category-2--5 hurricanes. These values are similar to ARCHER-2 errors with microwave or scatterometer data, and better than ARCHER-2 errors when only IR data are available. GeoCenter also performs skillful uncertainty quantification, producing a well calibrated ensemble of 150 TC-center locations. Furthermore, all predictors used by GeoCenter are available in real time, which would make GeoCenter easy to implement operationally every 10 min.</p></details> | <details><summary>Submi...</summary><p>Submitted to AMS journal Weather and Forecasting. Main body is 64 pages and 17 figures; supplement is another 33 pages and 31 figures</p></details> |
| **[Early Classification of Time Series: Taxonomy and Benchmark](http://arxiv.org/abs/2406.18332v5)** | 2025-04-08 | <details><summary>Show</summary><p>In many situations, the measurements of a studied phenomenon are provided sequentially, and the prediction of its class needs to be made as early as possible so as not to incur too high a time penalty, but not too early and risk paying the cost of misclassification. This problem has been particularly studied in the case of time series, and is known as Early Classification of Time Series (ECTS). Although it has been the subject of a growing body of literature, there is still a lack of a systematic, shared evaluation protocol to compare the relative merits of the various existing methods. This document begins by situating these methods within a principle-based taxonomy. It defines dimensions for organizing their evaluation, and then reports the results of a very extensive set of experiments along these dimensions involving nine state-of-the art ECTS algorithms. In addition, these and other experiments can be carried out using an open-source library in which most of the existing ECTS algorithms have been implemented (see https://github.com/ML-EDM/ml_edm).</p></details> |  |
| **[PATH: A Discrete-sequence Dataset for Evaluating Online Unsupervised Anomaly Detection Approaches for Multivariate Time Series](http://arxiv.org/abs/2411.13951v4)** | 2025-04-08 | <details><summary>Show</summary><p>Benchmarking anomaly detection approaches for multivariate time series is a challenging task due to a lack of high-quality datasets. Current publicly available datasets are too small, not diverse and feature trivial anomalies, which hinders measurable progress in this research area. We propose a solution: a diverse, extensive, and non-trivial dataset generated via state-of-the-art simulation tools that reflects realistic behaviour of an automotive powertrain, including its multivariate, dynamic and variable-state properties. Additionally, our dataset represents a discrete-sequence problem, which remains unaddressed by previously-proposed solutions in literature. To cater for both unsupervised and semi-supervised anomaly detection settings, as well as time series generation and forecasting, we make different versions of the dataset available, where training and test subsets are offered in contaminated and clean versions, depending on the task. We also provide baseline results from a selection of approaches based on deterministic and variational autoencoders, as well as a non-parametric approach. As expected, the baseline experimentation shows that the approaches trained on the semi-supervised version of the dataset outperform their unsupervised counterparts, highlighting a need for approaches more robust to contaminated training data. Furthermore, results show that the threshold used can have a large influence on detection performance, hence more work needs to be invested in methods to find a suitable threshold without the need for labelled data.</p></details> | <details><summary>Submi...</summary><p>Submitted to the Big Data Research journal</p></details> |
| **[Drought forecasting using a hybrid neural architecture for integrating time series and static data](http://arxiv.org/abs/2504.05957v1)** | 2025-04-08 | <details><summary>Show</summary><p>Reliable forecasting is critical for early warning systems and adaptive drought management. Most previous deep learning approaches focus solely on homogeneous regions and rely on single-structured data. This paper presents a hybrid neural architecture that integrates time series and static data, achieving state-of-the-art performance on the DroughtED dataset. Our results illustrate the potential of designing neural models for the treatment of heterogeneous data in climate related tasks and present reliable prediction of USDM categories, an expert-informed drought metric. Furthermore, this work validates the potential of DroughtED for enabling location-agnostic training of deep learning models.</p></details> | <details><summary>10 pa...</summary><p>10 pages, 3 figures, published as a workshop paper at Tackling Climate Change with Machine Learning at ICLR 2025, Tackling Climate Change with Machine Learning is a non-archival workshop</p></details> |

