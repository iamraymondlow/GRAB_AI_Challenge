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
</ul>
<ul>
    <strong>day</strong>: Day, where the value indicates the sequential order and 
                          not a particular day of the month.
</ul>
<ul>
    <strong>timestamp</strong>: Start time of 15-minute intervals, in the following
                                format: <hour>:<minute>, where hour ranges from 0 to 23 and 
                                minute is either one of (0, 15, 30, 45).
</ul>
<ul>
    <strong>demand</strong>: Aggregated demand normalised to be in the range [0,1].
</ul>

<h2>Python Packages</h2>
Please ensure that the following Python packages are installed on your computer 
before executing the code in the Jupyter notebooks.
<ul>pandas</ul>
<ul>Geohash</ul>
<ul>numpy</ul>
<ul>matplotlib.pyplot</ul>
<ul>seaborn</ul>
<ul>tqdm</ul>
<ul>random</ul>
<ul>pickle</ul>



