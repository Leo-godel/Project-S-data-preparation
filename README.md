# Project-S-data-preparation
Data preparation for Project-S ( Astronomy Project)

## Group member:
Zheyu Lu  
Rui Liu   
Shuqi Xu   

## Data Format
There are three datasets: 1_North_Europe.rar, 2_Brazil and 3_China.    
These datasets are named after the location of the observer. For example, 3_China is the dataset that records information observed from a location in China.     
Each dataset contains four file.   

### local_pos_on_earth
The png file called local_pos_on_earth.png records the observation point on earth, including the latitude and longtitude.   

### SunA, SunB
SunA.dat and SunB.dat records the observation information of SunA and SunB.    
For each file, the record follows the format below:
time direction_degree height_degree    
     
Time is the information recording the standard time (No time zone difference).   
Direction_degree is the information about azimuth angle of Sun observed from the location.   
height_degree is the information about altitude angle of Sun observed from the location.   

For time, the format is year month day hour min sec     
For direction_degree and height_degree, the format is degree minute second

### Moon
The format is almost the same with SunA and SunB.    
The only difference is there is an additional phase column, which is a number between 0 and 1, recording the moon phase.

