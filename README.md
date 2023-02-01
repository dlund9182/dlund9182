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

'Mount Saint Elias': 0.6953232419413998

'Cerro Arenales': 0.6842534178430452 

'Lautaro': 0.6618167587959637

'Monte San Valentín': 0.648723514893179

'Mount Logan': 0.5989780981323864

'Mount Fairweather': 0.5955955811238083

'Mount Crillon': 0.5632098322245664

'Mawson Peak': 0.5628498845362963

'Denali': 0.5337741671011101

'Aconcagua': 0.5336217702065112

'Mount Paget': 0.5322510311333338

'Cerro Torre': 0.5159122838015424

'Ismoil Somoni Peak': 0.49665125696291534

'Jengish Chokusu': 0.4953066766311222

'Kangchenjunga': 0.4909758968686672

'Dhaulagiri': 0.4756216941531952

'Nanga Parbat': 0.470521988995217

'Mount Cook': 0.4658549084384747

'Namcha Barwa': 0.46326860339419546

'Nanda Devi': 0.45991623928847764

'Mount Rainier': 0.45972293648552126

'Vinson Massif': 0.4589634594266044

'K2': 0.4521689936152209

'Mount Marcus Baker': 0.44066734049738754

'Annapurna': 0.4390414786134049

'Baintha Brakk': 0.43627910689536264

'makalu': 0.43245726444215826

'Mount Everest': 0.42994918058173526

'Rakaposhi': 0.42913008337303377

'Jannu': 0.42803872141711113

'Masherbrum': 0.42218276946507977

'Latok': 0.42140149834759305 

'Mount Elbrus': 0.41685854047041926

'Manaslu': 0.41570621516687806

'Kangto': 0.41388038677346967

'Lhotse': 0.41217019703526686

'Khiangyang Kish': 0.40960776415129657

'Lhotse Shar': 0.4012373599973283

'Nuptse': 0.3767631739903061

'Mount Ratz': 0.3741035405545543

'Hvannadalshnúkur': 0.3613736519111224

'Mount Hood': 0.35793515084835076

'Mount Baker': 0.35327280944837697

'Changabang': 0.3477598808917406

'Mount Waddington': 0.34101539421144667

'Mont Blanc': 0.3371933099462363

'Glacier Peak': 0.33343744089008337

'Mount Tutoko': 0.3303934677119538

'Mount Jefferson': 0.3170018644250131

'Mount Shasta': 0.30522902625959075

'Gunnbjørn Fjeld': 0.2954684448599408

'Huascarán': 0.2950449987343678

'South Sister': 0.2932200730568169

'Mount Cleveland': 0.2919388984490341

'Grand Teton': 0.2909517069988931

'Mount Silverthrone': 0.2852378496224654

'Chimborazo': 0.2815060654075989

'Gannett Peak': 0.26557355847821434

'Pico Cristóbal Colón': 0.2648940336746271

'Cloud Peak': 0.2621820587844304

'Mount Olympus': 0.2607233876860353

'Mount Robson': 0.23601697655904372

'Mount Elbert': 0.22960666179282252

'Golden Hinde': 0.22673689561081822

'Nevado del Ruiz': 0.2257505413670131

'Borah Peak': 0.22252300795470392

'Kings Peak': 0.21948670328342193

'Sacajawea Peak': 0.21608896830805854

'Mount Washington': 0.21490427873475593

'Mount Assiniboine': 0.21047403876231618

'Iconoclast Mountain': 0.19994665767033296

'Mount Lyell': 0.19858338971348255

'Mount Goddard': 0.19489491659794897

'Mount Ritter': 0.19446721498232403

'Mount Whitney': 0.19303235157907275

'Puncak Jaya': 0.18923268512198232

'Thompson Peak': 0.16538736441016907

'Marys Peak': 0.113220102168773

'Saddle Mountain': 0.1010210713306618

'Farallones de Cali': 0.05563971399011978

-------------
So the mountains of the Saint Elias range, the Northern and Southern Patagonia Icecaps dominate in the top spots for worst weather. They have the most consistent combination of cold weather, heavy precipitation and high winds. Now I noticed that for one of the forecasting sites, only temperature was fairly accurate. For
precipitation and especially winds it was very inaccurate or at least when compared to the observable real forecasts for Mount Washington. So therefore
for the above calculations I only included temperature data from that website.


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
