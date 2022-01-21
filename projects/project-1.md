---
layout: project
type: project
image: images/micromouse.jpg
title: COVID Data Representation
permalink: projects/covid_data_representation
# All dates must be YYYY-MM-DD format!
date: 2020-03-14
labels:
  - Java
  - Eclipse
summary: An ICS project that used Java to pull data from Excel spreadsheet and represent covid-19 metrics
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/covidHistogram.png">
  <img class="ui image" src="../images/covidTable.png">
</div>

During the coronavirus pandemic in early 2020, the Centers for Disease Control and Prevention (CDC) was constantly releasing daily data regarding the state of all 50 U.S states and U.S territories. For an ICS 111 assignment, we were tasked with a file with this data as input, scanning it and extracting the desired numbers, and representing them in a readable, organized fashion. The files were taken directly from the CDC website and read locally from our computers. I intend to work on the code in the future so that there is some sort of live data collection, but as of right now, the project only works with downloaded files with set dates and statistics. 

Code wise, the project is somewhat simple, but it was my first time connecting something outside of code itself and displaying it in a better format. Additionally, it was and still is relevent to the current uncertain state of the pandemic. The code takes a user inputted date to draw from the data file. A scanner then finds and reads the file, storing the appropiate values from certain columns. It then runs the information through a printTable function, which handles all the abbreviations, spacing, and formatting for the table. Similarly, the histogram goes through the same process, except it only accounts of daily cases at any given date for all states and territories. 

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```




