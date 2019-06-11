<h1> GRAB AI for SEA Challenge (Traffic Management) </h1>

This page contains the instruction needed to properly run the code
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
                                    format: <hour>:<minute>, where hour ranges from 0 to 23 and 
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
    <li>pandas</li>
    <li>Geohash</li>
    <li>numpy</li>
    <li>matplotlib.pyplot</li>
    <li>seaborn</li>
    <li>tensorflow</li>
    <li>tqdm</li>
    <li>random</li>
    <li>pickle</li>
</ul>

<h2>Training the model</h2>
The steps to training the model are as follows:
<ol>
    <li>
        Paste the training data into the same directory as the model_train.ipynb file,
        and ensure that it has the following file name: "training.csv".
    </li>
    <li>
        Open the model_train.ipynb file.
    </li>
    <li>
        Click on the "Kernel" tab on the top navigation bar and select "Restart 
        and Run All".
    </li>
    <li>
        At the end of the training process, the trained models will be stored
        in a separate folder named "models". Several pickle files will also
        be created to ensure data persistance.
    </li>
</ol>

<h2>Testing the model</h2>
The steps to testing the model are as follows:
<ol>
    <li>
        Click on the following Dropbox <a href=https://www.dropbox.com/s/d0b9zhdfrwisjmh/GRAB_AI_Challenge.zip?dl=0>link</a> 
        to download a zipped folder containing all of the pre-trained models, 
        pickle files and source code.
    </li>
    <li>
        Unzip the folder and paste the test data into the same directory as the 
        model_test.ipynb file.
    </li>
    <li>
        Open the model_test.ipynb file and replace "validation.csv" with the file
        name of the test data, under the "Import test data" section.
    </li>
    <li>
        Click on the "Kernel" tab on the top navigation bar and select "Restart 
        and Run All".
    </li>
    <li>
        Wait for the evaluation to be completed and review the test results.
    </li>
</ol>





