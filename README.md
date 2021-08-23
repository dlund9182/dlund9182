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

For a location to be considered it has to have weather forecast info from both websites so Dome A actually isn't considered since I only have weather forecast date from one 
website.  So here are the current results from the data I have so far. Keep in mind that this hasn't been even a full year of data and since as of this writing its Summer in 
Northern Hemisphere and Winter in the Southern Hemisphere, mountains in the Southern Hemisphere come out on top as having the worst weather but once it hits fall in Northern 
Hemisphere the results would start to switch in favor of the Northern Hemisphere. Thats why to really make a more objective assesment we really do need a number of full years 
of data. Well anyway here is what the data says so far for the worst wealther in the world

'Lautaro': 0.5839966812291904, 

'Cerro Arenales': 0.5686615711434276,

'Mawson Peak': 0.5604979354687009, 

'Monte San Valentín': 0.5277940656840031, 

'Cerro Torre': 0.45834995535068696, 

'Mount Paget': 0.42413778845636463, 

'Mount Saint Elias': 0.41434052324392995,

'Vinson Massif': 0.41278974125080065, 

'Aconcagua': 0.4025622173164484, 

'Annapurna': 0.3981102014462882,

'Denali': 0.39791830095472197, 

'K2': 0.3932439321148293, 

'Namcha Barwa': 0.38980445914801426, 

'Mount Cook': 0.38891930598338104, 

'Mount Fairweather': 0.3806918848988934, 

'Ismoil Somoni Peak': 0.379181605997627, 

'Mount Logan': 0.37799745593328, 

'Dhaulagiri': 0.3755345391200096, 

'Jengish Chokusu': 0.37421569821880674, 

'Mount Elbrus': 0.37343693135090095,

'Kangchenjunga': 0.3693020647352248, 

'Nanga Parbat': 0.3692609967939829, 

'Manaslu': 0.3558926475236906,

'Nanda Devi': 0.3531732340264602, 

'Mount Tutoko': 0.3490441801993935,

'Mount Crillon': 0.3483387786630449,

'Mount Rainier': 0.3462356207803758, 

'Mount Everest': 0.34082437151711903, 

'makalu': 0.3158255676920205, 

'Mont Blanc': 0.3087787889265296, 

'Jannu': 0.3080605740872148,

'Mount Marcus Baker': 0.2984928402335727, 

'Mount Ratz': 0.29620423190290956, 

'Lhotse': 0.2960938656198104, 

'Rakaposhi': 0.2958133733806144, 

'Khiangyang Kish': 0.29391339197264, 

'Baintha Brakk': 0.29387838066160943,

'Lhotse Shar': 0.2896102205013981, 

'Chimborazo': 0.28912315431318997, 

'Mount Hood': 0.28853229683665704, 

'Latok': 0.2850239377724168, 

'Masherbrum': 0.2848313800001519, 

'Kangto': 0.28295880178403526, 

'Mount Waddington': 0.28130076682936717,

'Mount Cleveland': 0.2700786393782142,

'Nuptse': 0.2695213641417501, 

'Cloud Peak': 0.26922904109267104,

'Changabang': 0.2679328247611158, 

'Mount Jefferson': 0.2590775093884838, 

'Mount Baker': 0.2575771516279915,

'Gannett Peak': 0.2566615067908708,

'Huascarán': 0.25598109163446636, 

'Gunnbjørn Fjeld': 0.2528463435964759, 

'Mount Silverthrone': 0.2523266429828119, 

'South Sister': 0.2513106850969056, 

'Hvannadalshnúkur': 0.25067341394441484,

'Pico Cristóbal Colón': 0.24998989711106237,

'Kings Peak': 0.24809918243533566, 

'Mount Shasta': 0.24296329659321944,

'Nevado del Ruiz': 0.24278564759608975,

'Farallones de Cali': 0.24260562772853475, 

'Grand Teton': 0.23681733505608982, 

'Puncak Jaya': 0.23062137098175042, 

'Marys Peak': 0.22552339113183661, 

'Mount Washington': 0.22117050416368075, 

'Mount Olympus': 0.22015967613213397, 

'Mount Elbert': 0.21421071596620847, 

'Nevado del Huila': 0.21084367510493596,

'Mount Ritter': 0.20766862631496744, 

'Mount Lyell': 0.19790529764075285, 

'Sacajawea Peak': 0.19186800947656976,

'Golden Hinde': 0.1912444146040957, 

'Mount Goddard': 0.19083632121652175, 

'Borah Peak': 0.18989513771907637, 

'Iconoclast Mountain': 0.1885471392828175, 

'Mount Robson': 0.18797290356531635, 

'Mount Assiniboine': 0.18318304181369285, 

'Glacier Peak': 0.17488623867849287,

'Mount Whitney': 0.16522579235533952, 

'Saddle Mountain': 0.15829685395933538,

'Thompson Peak': 0.15120693071016292

The top 6 are all in the Southern Hemisphere which is to be expected given its August 22nd as of this writing. Note that Mount Saint Elias is in the number 7th spot even 
though its in the Northern Hemisphere so this maybe a pretty good indicator that Mount Saint Elias might consistently have one of the worst weather in the world regardless of 
which time of year it is. There might be other locations on glaciers (I'm thinking in particular of the Southern Patagonia Icefield) that have even worst weather but there is 
no weather forecasting websites that give data for those locations.


Note what Mount Washington is rather low in terms of its rating despite how often its cited as supposedly the worst weather in the world despite the fact it has no glaciation on the mountain and there is road going all the way up to the summit.



But more generally what am I interested in? In the short term anything related to Python but am interested in other languages as well like Java, C++ and Maybe Haskell. In the 
long run Data science and possibly Machine learning especially in the context of better understanding scientific  issues(in particular as it relates to Climate and weather 
forecasting in extreme weather enviroments).  I'm in particular trying to find some kind of python module that can give reliable climate data based on latitude and longitude 
for South America simuilar to what http://www.climatewna.com/ does for North America. I know of one window based piece of software but the precipiation data is really 
unreliable for the part of the South America I'm interestedin(North and South Patagonia Icefield). I also know of https://spotwx.com/ but that gives forecast info for 
elevations that are lower than the actual elevation for a latitude/longitude pair.

I also would to do something similar with air quality for National Parks and wilderness areas.

<!---
dlund9182/dlund9182 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
