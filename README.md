<h1> GRAB AI for SEA Challenge (Traffic Management) </h1>

This section contains the instructions needed to properly run the code
written for the GRAB AI for SEA Challenge 2019 (Traffic Management).

<h2> Data Description </h2>
The given dataset contains normalised historical demand of a city, 
aggregated spatiotemporally within geohashes and over 15 minute 
intervals. The dataset spans over a two month period. A brief 
description of the dataset fields are found below:

<ul>
    <li>
        <strong>geohash6</strong>: Geohash is a public domain geocoding system which 
                                   encodes a geographic location into a short string of letters 
                                   and digits with arbitrary precision. You may use the Python 
                                   Geohash package https://pypi.org/project/Geohash/ or any Java 
                                   Geohash library https://github.com/kungfoo/geohash-java or 
                                   similar to encode and decode geohash into latitude and longitude
                                   and vice versa.
    </li>
    <li>
        <strong>day</strong>: Day, where the value indicates the sequential order and 
                              not a particular day of the month.
    </li>
    <li>
        <strong>timestamp</strong>: Start time of 15-minute intervals, in the following
                                    format: hour:minute, where hour ranges from 0 to 23 and 
                                    minute is either one of (0, 15, 30, 45).
    </li>
    <li>
        <strong>demand</strong>: Aggregated demand normalised to be in the range [0,1].
    </li>
</ul>

<h2>Python Packages</h2>
Please ensure that the following Python packages are installed on your computer 
before executing the code in the Jupyter notebooks: 

<ul>
    <li><strong>pandas</strong></li>
    <li><strong>Geohash</strong></li>
    <li><strong>numpy</strong></li>
    <li><strong>matplotlib.pyplot</strong></li>
    <li><strong>seaborn</strong></li>
    <li><strong>tensorflow</strong></li>
    <li><strong>tqdm</strong></li>
    <li><strong>random</strong></li>
    <li><strong>pickle</strong></li>
</ul>

<h2>Training the model</h2>
<ol>
    <li>
        Paste the training data into the same directory as the <strong>model_train.ipynb</strong> file,
        and ensure that it has the following file name: <strong>training.csv</strong>.
    </li>
    <li>
        Open the <strong>model_train.ipynb</strong> file.
    </li>
    <li>
        Click on the <strong>Kernel</strong> tab on the top navigation bar and select <strong>Restart 
        and Run All</strong>.
    </li>
    <li>
        At the end of the training process, the trained models will be stored
        in a separate folder named <strong>models</strong>. Several pickle files will also
        be created to ensure data persistance.
    </li>
</ol>

<h2>Testing the model</h2>
<ol>
    <li>
        Drop me an e-mail at the following address: <a href=iamraymondlow@gmail.com>
        iamraymondlow@gmail.com</a>  and I will send you a zipped folder containing all of the pre-trained models, 
        pickle files and source code.
    </li>
    <li>
        Unzip the folder and paste the test data into the same directory as the 
        <strong>model_test.ipynb</strong> file.
    </li>
    <li>
        Open the <strong>model_test.ipynb</strong> file and replace <strong>validation.csv</strong> with the file
        name of the test data, under the <strong>Import test data</strong> section.
    </li>
    <li>
        Click on the <strong>Kernel</strong> tab on the top navigation bar and select <strong>Restart 
        and Run All</strong>.
    </li>
    <li>
        Wait for the evaluation to be completed and review the test results.
    </li>
</ol>





