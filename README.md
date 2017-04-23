# Luminescence: LifeBand Website (nwHacks 2017)

A distributed and scalable software system designed chiefly to alleviate patient misidentification in hospitals and senior centers.

![Lifeband Logo](logo.png)

## The Inspiration and Problem

According to a study by the esteemed Johns Hopkins University, the third leading cause of death in the US is [patient misidentification](https://www.washingtonpost.com/news/to-your-health/wp/2016/05/03/researchers-medical-errors-now-third-leading-cause-of-death-in-united-states/). Over a quarter of a million people die annually due to preventable medical errors - that's 700 deaths a day, or 1 death every two minutes.

## The Solution

Our solution was to create an inexpensive solution which could be scaled to the needs of an entire country's medical records and would allow for maximum availability even when under immense usage. The software system would also allow for complex data analytics to be performed, resulting in a significant increase in medical statistics.

### The System and Technologies

Inexpensive and small identification tags which emit [NFC](http://electronics.howstuffworks.com/nfc-tag.htm) are attached to hospital beds, or placed on wristbands and given to residents of senior centers. These are registered with the records of the person they are given to.

Users interact with the tags by opening an Android application and scanning the tag with their NFC-enabled device. The application will contact a [Golang](https://golang.org/) server which will query a [CockroachDB](https://github.com/cockroachdb/cockroach) database, both of which are hosted on [Amazon Web Services](https://aws.amazon.com/). The patient data returned will be displayed on the device.

### Lightning Talk Presentation

[![YouTube preview image](http://img.youtube.com/vi/gbXAl5zKDpA/maxresdefault.jpg)](https://www.youtube.com/watch?v=gbXAl5zKDpA/)
