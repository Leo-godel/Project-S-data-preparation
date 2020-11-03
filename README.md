# Project-S-data-preparation
Data preparation for Project-S (Astronomy Project)

## Group member:
Zheyu Lu
Rui Liu
Shuqi Xu

## Data Format
There are three datasets: 1_Berkeley.rar, 2_Shanghai.rar, and 3_Sydney.rar. In each of these compressed file, you will find four files: Moon.dat, Sun_A.dat, Sun_B.dat, and local_pos_on_earth.png.

These datasets are named after the location of the observer. For example, 2_Shanghai contains data observed by an observer whose location is roughly at Shanghai, China. The exact longitude and latitude information of the observer can be found in local_pos_on_earth.png.

There is also a text file called Raw_picture_data.txt, which contains a link to the raw picture data we used to generate these information.

### local_pos_on_earth
The png file called local_pos_on_earth.png records the observation point on earth, including the latitude and longtitude.

### Sun_A, Sun_B
Sun_A.dat and Sun_B.dat contains the observation information of the two stars SunA and SunB in our binary star solar system.
For each file, the record follows the format below:
Figure index, Time, Direction(azimuthal angle), Height(polar angle), Apparent size

1. Figure index indicates the corresponding figure for generating this line of data.
2. Time is the absolute time in our fictional universe(No time zone difference).
3. Direction is the azimuthal angle of the Sun observed from the given location in spherical coordinates.
4. Height is the polar angle of the Sun observed from the given location in spherical coordinates.

For Time, the format in the file is: year month day hour minute second
For Direction, Height, and Apparent size, the format in the file is: degree minute second

### Moon
The format is the same as that of Sun_A.dat and Sun_B.dat except that there is an additional data column recording the phase of moon.
The phase of moon should be a number between 0 and 1. However, due to the not high recognition rate of the Optical Character Recognition(OCR) package we are using, this column contains some invalid data.

