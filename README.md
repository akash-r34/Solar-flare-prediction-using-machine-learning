# Solar flare prediction using machine learning

<h3>Team members</h3>
<ul>
<li><b>AKASH R 20BCE1501</b> Github: <a href="https://github.com/akash-r34">akash-r34</a></li>
<li><b>ABRAR AHAMED 20BCE1437</b> Github: <a href="https://github.com/Abrar-Ahamed">Abrar-Ahamed</a></li>
</ul>

<h2>Abstract</h2>

<p>This project focuses on predicting solar flare peak current per second (c/s) and energy magnitude using a variety of recurrent neural network architectures, including LSTM, GRU, and Bidirectional LSTM + GRU. Through systematic hyperparameter tuning, we aim to optimize model performance, offering an advanced tool for forecasting solar activities with enhanced accuracy and reliability. The project is implemented in a modular and transparent manner, making it a valuable resource for researchers and practitioners in the field of space weather prediction. The codebase is available on GitHub, providing an accessible platform for further exploration and collaboration.</p>


<pre>
├── Dataset
│   └── hessi.solar.flare.2002to2016.csv
├── Code
│   └── solar_flare_prediction.ipynb
├── Results
│   └── (various model outputs and visualizations)
├── README.md
└── requirements.txt
</pre>

<h2>Getting Started</h2>

<p>To run the code, make sure you have the required dependencies installed. You can install them using the following command:</p>

<code>pip install -r requirements.txt</code>

<p>Open the Jupyter Notebook <code>solar_flare_prediction.ipynb</code> to explore the code and run the machine learning models.</p>

<h2>Data Collection</h2>

<p>The dataset is collected by utilizing SHARP summary parameters as input data for the prediction model. SHARPs are derived from vector magnetograms captured by the HMI on the SDO. Summary parameters are computed based on the HMI Active Region (AR) patches (HARPs), which are rectangular boxes encompassing the ARs and moving with solar rotation.</p>

<ul>
    <li><strong>Data Source:</strong> Joint Science Operations Center (JSOC) - <a href="http://jsoc.stanford.edu">http://jsoc.stanford.edu</a></li>
    <li><strong>Time Range:</strong> 2002 to 2016</li>
</ul>

<h3>Solar Flare Event Identification</h3>

<p>Solar flare events are identified using the NOAA Geostationary Operational Environmental Satellite (GOES) flare list. The GOES flare list includes flare events with class, start, end, and peak intensity times for each event. The peak time of the flare events is designated as the "event time" when constructing the data samples for the prediction model.</p>



<h2>Dataset Information</h2>

<p>The dataset contains information about solar flares, including peak count rates, total counts, energy levels, and various flags indicating flare characteristics.</p>

<h2>Machine Learning Models</h2>

<p>The project includes the following machine learning models:</p>

<ul>
<li>LSTM model for predicting 'peak.c/s'</li>
<li>GRU model for predicting 'energy.keV'</li>
<li>Combined LSTM and GRU model for predicting flare categories</li>
<li>Hyperparameter tuning and custom-weighted loss function</li>
<li>Bidirectional LSTM and GRU model for predicting flare categories</li>
</ul>

<h2>Results</h2>

<p>Various visualizations and evaluation metrics are provided in the Jupyter Notebook to assess the performance of the models.</p>

<h2>Contributing</h2>

<p>Feel free to contribute to this project by opening issues or submitting pull requests. Your feedback and contributions are highly appreciated!</p>


