# Rachel Chong's Brainstation Capstone - U.S. Accidents

### Project Overview
**Problem Area:** My area of interest lies in leveraging data science and machine learning to improve road safety and mitigate accidents. Within this domain, there are numerous challenges to address, including identifying accident hotspots, predicting accidents in real-time, understanding the causative factors contributing to accidents, and studying the impact of various environmental stimuli on accident occurrence.

**The User:** The individuals affected by these problems span a wide spectrum, including commuters, law enforcement agencies, emergency services, city planners, and insurance companies. Commuters would benefit from reduced accident risks and improved travel times. Law enforcement and emergency services would gain insights for better resource allocation and response strategies. City planners could use the outcomes to design safer roads, and insurance companies could refine their risk assessment models.

**Big Idea:** Machine learning offers a robust framework to tackle these challenges. Techniques such as predictive modeling can forecast accident occurrences based on historical data and current conditions. Clustering algorithms can identify accident hotspots, while causal inference methods can extract cause-and-effect rules to predict accidents. Previous approaches in this field have utilized regression models, decision trees, neural networks, and ensemble methods to address similar problems.

**The Impact:** The societal impact of reducing accidents through improved predictive models and better understanding of causative factors is substantial. In the United States alone, accidents incur billions of dollars in costs annually due to property damage, medical expenses, lost productivity, and legal ramifications. Moreover, the human toll in terms of injuries and fatalities is immeasurable. By accurately predicting accidents and implementing preventive measures, the potential for reducing these costs and saving lives is immense.

**The Data:** The "US-Accidents" dataset covering 49 states in the USA from February 2016 to March 2023, containing approximately 7.7 million accident records, is a comprehensive resource for this project. This dataset encompasses various aspects of accidents, including location, severity, weather conditions, time of day, and more, sourced from multiple entities such as transportation departments, law enforcement, cameras, and sensors. Additionally, supplementary datasets like weather records, road network information, and traffic patterns could complement the analysis and enrich the predictive models.

Beyond this dataset, complementary sources such as the National Highway Traffic Safety Administration (NHTSA) Crash Report database or state-specific accident records could further enhance the understanding of accident patterns and contributing factors, offering a more holistic approach to the project.

The "US-Accidents" dataset covers accidents across the USA in detail. It includes accident IDs, severity levels, timestamps, GPS coordinates, road length affected, weather data (temperature, humidity, precipitation), and descriptions. Additionally, it notes nearby Points of Interest (POIs) like crossings, traffic signals, and weather conditions categorized by twilight phases and day/night periods. This detailed information allows for a multidimensional analysis to understand accident contexts, aiding predictive modeling and road safety initiatives.

The following table describes the data attributes:

| Attribute             | Description                                                                                           | Nullable |
|-----------------------|-------------------------------------------------------------------------------------------------------|----------|
| ID                    | Unique identifier of the accident record                                                               | No       |
| Severity              | Severity of the accident on a scale of 1 to 4 where 1 indicates minimal impact and 4 significant     | No       |
| Start_Time            | Start time of the accident in local time zone                                                          | No       |
| End_Time              | End time of the accident in local time zone; dismissal of impact on traffic flow                       | No       |
| Start_Lat             | Latitude in GPS coordinate of the start point                                                          | No       |
| Start_Lng             | Longitude in GPS coordinate of the start point                                                         | No       |
| End_Lat               | Latitude in GPS coordinate of the end point (Nullable)                                                 | Yes      |
| End_Lng               | Longitude in GPS coordinate of the end point (Nullable)                                                | Yes      |
| Distance(mi)          | Length of the road extent affected by the accident                                                     | No       |
| Description           | Natural language description of the accident                                                           | No       |
| Number                | Street number in address field (Nullable)                                                              | Yes      |
| Street                | Street name in address field (Nullable)                                                                | Yes      |
| Side                  | Relative side of the street (Right/Left) in address field (Nullable)                                   | Yes      |
| City                  | City in address field (Nullable)                                                                       | Yes      |
| County                | County in address field (Nullable)                                                                     | Yes      |
| State                 | State in address field (Nullable)                                                                      | Yes      |
| Zipcode               | Zipcode in address field (Nullable)                                                                    | Yes      |
| Country               | Country in address field (Nullable)                                                                    | Yes      |
| Timezone              | Timezone based on the location of the accident (Nullable)                                              | Yes      |
| Airport_Code          | Denotes the closest airport-based weather station to the accident location                             | Yes      |
| Weather_Timestamp     | Time-stamp of weather observation record (in local time)                                                | Yes      |
| Temperature(F)        | Temperature in Fahrenheit                                                                             | Yes      |
| Wind_Chill(F)         | Wind chill in Fahrenheit                                                                              | Yes      |
| Humidity(%)           | Humidity percentage                                                                                    | Yes      |
| Pressure(in)          | Air pressure in inches                                                                                 | Yes      |
| Visibility(mi)        | Visibility in miles                                                                                    | Yes      |
| Wind_Direction        | Wind direction                                                                                         | Yes      |
| Wind_Speed(mph)       | Wind speed in miles per hour                                                                           | Yes      |
| Precipitation(in)     | Precipitation amount in inches, if any                                                                 | Yes      |
| Weather_Condition     | Weather condition (rain, snow, thunderstorm, fog, etc.)                                                 | Yes      |
| Amenity               | Presence of amenity in a nearby location                                                               | No       |
| Bump                  | Presence of speed bump or hump in a nearby location                                                    | No       |
| Crossing              | Presence of crossing in a nearby location                                                              | No       |
| Give_Way              | Presence of give_way in a nearby location                                                              | No       |
| Junction              | Presence of junction in a nearby location                                                              | No       |
| No_Exit               | Presence of no_exit in a nearby location                                                               | No       |
| Railway               | Presence of railway in a nearby location                                                               | No       |
| Roundabout            | Presence of roundabout in a nearby location                                                            | No       |
| Station               | Presence of station in a nearby location                                                               | No       |
| Stop                  | Presence of stop in a nearby location                                                                  | No       |
| Traffic_Calming       | Presence of traffic_calming in a nearby location                                                       | No       |
| Traffic_Signal        | Presence of traffic_signal in a nearby location                                                        | No       |
| Turning_Loop          | Presence of turning_loop in a nearby location                                                          | No       |
| Sunrise_Sunset        | Period of day (day or night) based on sunrise/sunset                                                   | Yes      |
| Civil_Twilight        | Period of day (day or night) based on civil twilight                                                   | Yes      |
| Nautical_Twilight     | Period of day (day or night) based on nautical twilight                                                | Yes      |
| Astronomical_Twilight | Period of day (day or night) based on astronomical twilight                                            | Yes      |


