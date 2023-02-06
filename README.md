Hi  

My Name is Dennis. I currently have only one repository which is a repository of python code that parses weather data from websites that give weather forecasts for mountains 
some of which are rather remote. The script stores the data in a database(actually it was two databases until the Mysql database stopped working).  The goal is to give enough 
data(at least 10 years worth of data) so I can get a better idea of which mountains get the most precipitation and snow which I suspect  will be either the Saint Elias Range
(more specifically the southern part of the range known as the Fairweather range) and various locations in the Southern Patagaonia Icefield.  I started this python scraping
script in mid February of 2021 so that means I have weather forecast data starting from mid February of 2021 but have added additional locations in April and May.  Starting 
January 1st of 2022 I will erase the data and start from scratch since I want the locations to all start on the same day and be judged by entire years.

I also want to have an idea of what areas have the worst weather in the world. To that end I have a specific script that uses data from two websites to try and figure out 
where is the worst weather in the world. It uses temperature,precipitation/snowfall and wind equally to determine this. Now its an assumption on my part that I'm treating 
temperature, precipitation/snowfall and wind equally. Maybe one should be viewed as more important than the others but at this time I have no reason to believe this is the
case. So I use two different websites to determine temperature and wind speed. One website for snowfall and rain data and another for precipitation. It gives a float number 
between 0 and 1 for each mountain. A 1 would be considered the worst possible weather which would mean it would have the coldest temperature, most precipitation/snowfall and 
the windiest locations as well. Note that it would be impossible for any location to get a 1 because there is an inverse relationship between heavy precipitation and how cold 
a place is. Really cold places like Dome A in Antartica are very dry because at really cold temperatures they just can't hold a lot of precipitation.  In addition a really 
cold place like Dome A has very little wind. On the other end of the spectrum a 0 would be considered the exact opposite of the worst weather in the world. 

For a location to be considered it has to have weather forecast info from both websites so Dome A actually isn't considered since I only have weather forecast data from one 
website.  So here are the current results from the data I have so far. Keep in mind that this hasn't been even a full year of data and as of this writing its Summer in 
Northern Hemisphere and Winter in the Southern Hemisphere, mountains in the Southern Hemisphere come out on top as having the worst weather but once it hits fall in Northern 
Hemisphere the results would start to switch in favor of the Northern Hemisphere. Thats why to really make a more objective assesment we really do need a number of full years 
of data. Well I actually do have a full years worth of Data for 2022 and here are the results


'Mount Saint Elias': 0.6761311594690332

'Cerro Arenales': 0.6437360402220347

'Lautaro': 0.6236424643860942

'Monte San Valentín': 0.6126843724649843

'Mount Logan': 0.582692122552209

'Mount Fairweather': 0.5673970758779551

'Mount Crillon': 0.5284419763882667

'Mawson Peak': 0.5254876598456868

'Denali': 0.5221914299722641

'Aconcagua': 0.5075679642368424

'Mount Paget': 0.49534775182214713

'Jengish Chokusu': 0.47986898764757174

'Ismoil Somoni Peak': 0.47914726464341123

'Cerro Torre': 0.4738045424146408

'Kangchenjunga': 0.47040501369037885

'Vinson Massif': 0.4538413375182156

'Nanga Parbat': 0.4534010747769039

'Dhaulagiri': 0.4521389397777618

'K2': 0.44130605416082586

'Namcha Barwa': 0.43649712022320425

'Nanda Devi': 0.4361664261863536

'Mount Cook': 0.4213976632006064

'Mount Rainier': 0.41956354429654685

'Baintha Brakk': 0.41463669079872373

'Annapurna': 0.4140920527517072

'Mount Everest': 0.41152044926595494

'makalu': 0.4100600835473882

'Mount Marcus Baker': 0.40954927289963683

'Rakaposhi': 0.40919057921726737

'Masherbrum': 0.40691833698948593

'Jannu': 0.3994076073316992

'Latok': 0.3985624491129971

'Khiangyang Kish': 0.3923430577206937

'Manaslu': 0.39112830546408883

'Lhotse': 0.39108265952876226

'Mount Elbrus': 0.3861956869307232

'Lhotse Shar': 0.3790843348107434

'Kangto': 0.37871801972445857

'Nuptse': 0.3502687755468646

'Mount Ratz': 0.33240023470531893

'Changabang': 0.31583694173059296

'Hvannadalshnúkur': 0.3148535000109236

'Mount Hood': 0.3086859088458675

'Mount Baker': 0.30558459842951696

'Mount Waddington': 0.3013399795791382

'Mont Blanc': 0.2985146058092405

'Glacier Peak': 0.28498966750384763

'Mount Tutoko': 0.2784351979089756

'The real mount Washington': 0.2725707523386968   # Based on real observable data for 2022. NOT based on modeled forecasts

'Mount Jefferson': 0.26482900220652333 

'Gunnbjørn Fjeld': 0.2614645127527599

'Mount Shasta': 0.2587416024321398

'Huascarán': 0.2526538152222671

'Grand Teton': 0.24648344143265688

'Mount Cleveland': 0.2432904007469685

'South Sister': 0.23963376815597584

'Mount Silverthrone': 0.23687006503875732

'Chimborazo': 0.23594039464953442

'Gannett Peak': 0.22066513504074545

'Pico Cristóbal Colón': 0.21587685485786015

'Cloud Peak': 0.21561916736689826

'Mount Olympus': 0.20571191734825897

'Mount Robson': 0.18436014103914264

'Mount Elbert': 0.18281097904847735

'Borah Peak': 0.17439896153719844

'Nevado del Ruiz': 0.17220577142455307

'Golden Hinde': 0.171728847036299

'Kings Peak': 0.1709589821347771

'Sacajawea Peak': 0.1620164394163018

'Mount Assiniboine': 0.160975703629703

'Mount Washington': 0.1592238363234412

'Iconoclast Mountain': 0.15079866489380703

'Mount Lyell': 0.14585300156561665

'Mount Goddard': 0.14315149423072915

'Mount Whitney': 0.14206526224691515

'Mount Ritter': 0.14151570244879252

'Puncak Jaya': 0.13212950358048353

'Thompson Peak': 0.10525486071327221

'Marys Peak': 0.047954955409605905

'Saddle Mountain': 0.03546852185316519

'Farallones de Cali': -0.006626890214159936

-------------
So the mountains of the Saint Elias range, the Northern and Southern Patagonia Icecaps dominate the top spots for worst weather. They have the most consistent combination of cold weather, heavy precipitation and high winds. Now I noticed that for one of the forecasting sites, only temperature was fairly accurate. For
precipitation and especially winds it was very inaccurate or at least when compared to the observable real forecasts for Mount Washington. So therefore
for the above calculations I only included temperature data from that website.

Well anyway for 2022 here is the actual real observed data for Mount Washington

From https://www.mountwashington.org/experience-the-weather/observer-comments.aspx?id=59057

average temperature = 29.3°F (-1.5°C), 
precipitation = 94 inches
Average Wind speed =  36.4 mph
Snowfall = 236.7 inches


Based on the weather scraped where I would take the daily average and then extrapolate to 365 since there were some days that were missing(but very few)

average temperature from YR = -2.4 C
average temperature from MountainForecast = 0.8 C
precipitation (from YR) = 69.3 inches
Snowfall(From MountainForecast) = 274.5 inches
average wind speed from MountainForecast = 20.2 MPH
average wind speed from YR = 6.5 MPH

So in this example the models for temperature were the most accurate but the models for Wind speed the least accurate.

Also there is information on the average annual temperature for Denali and Mount Rainier based on this website
https://www.summitpost.org/interesting-climate-statistics-for-us-mountain-summits/171585

The average temperature at the summit of Denali is -28 F(-33.3 C)
The average temperature at the summit of Mount Rainier is 11.9F(-11.2 C)

The data for 2022 when averaging the temp values for Denali and Rainier were as follows

Denali
YR has the average temp at -32.5 C
MountainForecast has it at -32.3 C

Mount Rainier
YR has the average temp at -12.45 C
MF has the average temp at - -11.3 C


But more generally what am I interested in? In the short term anything related to Python but am interested in other languages as well like Java, C++ and Maybe Haskell. In the 
long run Data science and possibly Machine learning especially in the context of better understanding scientific  issues(in particular as it relates to Climate and weather 
forecasting in extreme weather enviroments).  I'm in particular trying to find some kind of python module that can give reliable climate data based on latitude and longitude 
for South America similar to what http://www.climatewna.com/ does for North America. I know of one window based piece of software but the precipiation data is really 
unreliable for the part of the South America I'm interestedin(North and South Patagonia Icefield). I also know of https://spotwx.com/ but that gives forecast info for 
elevations that are lower than the actual elevation for a latitude/longitude pair.

I also want to do something similar with air quality for National Parks and wilderness areas.

<!---
dlund9182/dlund9182 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
