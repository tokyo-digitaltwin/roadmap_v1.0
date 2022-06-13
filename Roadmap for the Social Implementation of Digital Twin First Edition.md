## デジタルツインの社会実装に向けたロードマップ 初版 
2022年3月　東京都 

 ### 目次
 0. [Introduction](#anchor0)
 1. [Digital Twin Concept](#anchor1)  
 1.1[What is Digital Twin?](#anchor1.1)  
 1.2[Significance of Tokyo Digital Twin Initiative](#anchor1.2)  
 1.3[Tokyo Metropolitan Government's Initiatives Related to Digital Twin](#anchor1.3) 

 2. [Our goal through Digital Twin](#anchor2)  
2.1[Value of Digital Twin](#anchor2.1)  
2.2[What is the complete digital twin that we aim to realize?](#anchor2.2)  
 3. [Components of Digital Twin](#anchor3)  
  3.1[Overall Picture of Digital Twin](#anchor3.1)  
  3.2[Components of Digital Twin](#anchor3.2)  
  3.3[Components of Cyber Space](#anchor3.3)  
  3.4[Components of Physical Space](#anchor3.4)  
  3.5[Elements common to Cyber and Physical Space](#anchor3.5)  
  3.6[Other Factors](#anchor3.6)

 4. [Steps toward realizing Digital Twin](#anchor4)  
  4.1[Steps to realize Digital Twin](#anchor4.1)  
  4.2[Implementation of base elements](#anchor4.2)  
  4.3[Maintenance of ancillary elements](#anchor4.3)  
  4.4[Service Implementation](#anchor4.4)  
  4.5[Digital Twin area development](#anchor4.5)  

 5. [Maintenance and operation of Digital Twin](#anchor5)  
  5.1[Role and cost-sharing approach](#anchor5.1)  
  5.2[Division of roles in the development of Digital Twin](#anchor5.2)  
  5.3[Division of roles in the operation of Digital Twin](#anchor5.3)  

 6. [Cost-effectiveness of Digital Twin Development](#anchor6)  
  6.1[Approach to Estimating cost](#anchor6.1)  
  6.2[Approach to Estimating Effectiveness](#anchor6.2)  
  6.3[Example of cost-effectiveness expressions](#anchor6.3)  

 7. [Conclusion」](#anchor7)  
 [Reference Glossary](#anchor参考用語集)  
 [References](#anchor参考：参考文献)



<a  id="anchor0"></a>
<a  href="#anchor0"></a>
###  0. Introduction

The Japanese government has proposed "Society 5.0," a human-centered society that uses cutting-edge technology to achieve both economic development and solutions to social issues. The Ministry of Land, Infrastructure, Transport and Tourism (MLIT) has been working on the realization of a "super-smart society.

As part of this effort, MLIT is working on the development and open data creation of 3D city models nationwide under the Urban Digital Transformation (DX) project for urban development titled "Project PLATEAU.

The Tokyo Metropolitan Government, while aligning its vector with the efforts of the national government, has set forth the "Promotion of Digital Twin to Support the Realization of Smart Tokyo" in the "Smart Tokyo Implementation Strategy" released in February 2020. In addition, as related projects in FY2020, the "Preparatory Meeting for the Operation of a Public-Private Partnership Data Platform" consisting of experts and others, and the "Tokyo Metropolitan Government 3D Visualization Demonstration Project" were implemented with the aim of building a public-private cooperated data platform.

In this fiscal year (FY2021), in order to accelerate the social implementation of the urban digital twin, the "Study Group for Social Implementation of Urban Digital Twin in Tokyo" (hereinafter referred to as the "Study Group"), consisting of experts, was established. Based on a total of four discussions, the Study Group has examined the desirable way of proceeding with the construction of the urban digital twin and conducted a demonstration project to clarify technical issues.

Based on the discussions at the study group, this roadmap was designed to achieve these three goals, to define concrete steps and actions toward the development and utilization of an urban digital twin, to clarify the cost-effectiveness expected from the development of an urban digital twin, and to communicate these in an easy-to-understand manner to Tokyo residents and private businesses. The purpose of this roadmap is to clarify the cost-effectiveness of the development of the urban digital twin.

In order to realize the contents of this roadmap, we will make a concerted effort to promote the project with the cooperation of industry, academia, and government across organizations and fields.

<a  id="anchor1"></a>
<a  href="#anchor1"></a>
### 1. 1.	Digital Twin Concept

<a  id="anchor1.1"></a>
<a  href="#anchor1.1"></a>
### 1.1 1.1.	What is Digital Twin?

****▼Reproduce physical space in cyber space to build and utilize "twins“.****

As shown in Figure 1-1, a digital twin is a cyberspace (virtual space on a computer or computer network) that reproduces various elements like buildings, roads and other infrastructure, economic activities, and human flows as "twins" based on data acquired from sensors and other sources.

Based on real-time data obtained from activities in various fields in physical space (real space), advanced analysis and simulation are performed in cyber space (virtual space), and the results are fed back to physical space in a high-speed and interactive manner. Utilization of the digital twin refers to the state in which this continuous loop is realized.


<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%A8%E3%81%AF.png?raw=true" width="60%">

**Figure 1-1 What is Digital Twin?**

 
<a  id="anchor1.2"></a>
<a  href="#anchor1.2"></a>
### 1.2 Significance of Tokyo Digital Twin Initiative

****▼Japanese economic presence in the world is declining and the digital shift of Japan is lagging.****

As shown in Figure 1-2, China and India are projected to rank first and third in world GDP by 2030, with both countries' global share rising from 22% to 34%. Japan, on the other hand, is expected to fall from its current third place to fourth, and its presence in the world is declining. 

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-2%20%E5%AE%9F%E8%B3%AAGDP%E3%81%AE%E5%9B%BD%E5%88%A5%E3%82%B7%E3%82%A7%E3%82%A2%EF%BC%882010%E5%B9%B4%EF%BC%8F2030%E5%B9%B4%EF%BC%89.png?raw=true" width="60%">
(Source) Based on OECD, Economic Outlook No,95 (2014)<br>

**Figure 1-2　Real GDP Share by Country（2010/2030）**  <p>


In particular, in the field of digitalization where competition is thriving in many countries, Japan is ranked 27th overall in IMD's "Global Digital Competitiveness Ranking" (Figure 1-3), hardly a world leader.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-3%20%E4%B8%96%E7%95%8C%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E7%AB%B6%E4%BA%89%E5%8A%9B%E3%83%A9%E3%83%B3%E3%82%AD%E3%83%B3%E3%82%B0.png?raw=true" width="30%">
(Source) Based on IMD, World Digital Competitiveness Ranking<br>

**Figure 1-3　Global Digital Competitiveness Ranking**  <p>

****▼Declining birthrate, aging, declining population, and other factors have a significant impact on productivity and urban vitality of Japan. ****

Regarding the population that supports the economy shown in Figure 1-4, the proportion of the elderly population (aging rate) to the population of Tokyo in 2015 was 22.7%, indicating that the city has already entered a super-aging society.

The composition of Tokyo's population is expected to change drastically by 2060, with the juvenile population and working-age population decrease by approximately 30% and 20% compared to 2015.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-4%20%E6%9D%B1%E4%BA%AC%E9%83%BD%E3%81%AE%E5%B9%B4%E9%BD%A2%E9%9A%8E%E7%B4%9A%E5%88%A5%E4%BA%BA%E5%8F%A3.png?raw=true" width="60%">
<span style="font-size: 50%; color;">Source）Compiled from "Tokyo Metropolitan Government Daytime Population Projections (March 2020)" (Bureau of General Affairs, Tokyo Metropolitan Government), "National Census" (Ministry of Internal Affairs and Communications), etc.</span><br>
<span style="font-size: 50%; color;">（Remarks）1．The values after 2045 are estimated by Office of the Governor for Policy Planning, Tokyo Metropolitan Government</span><br>
<span style="font-size: 50%; color;">2．The value in parentheses in the breakdown is the percentage of the population.（The percentage in 2015 is calculated by dividing the unknown age into each age group.）</span><br>
<span style="font-size: 50%; color;">3．The total breakdown may not match the total number due to rounding and the actual value including unknown age.</span><br>
（Source）「Based on “Future Tokyo” Strategy, Annex<br>

**Figure 1-4　Population by age group in Tokyo**<p>

****▼Increasing frequency and severity of natural disasters and rising risk of earthquakes directly under the Tokyo metropolitan area.****

Regarding natural disasters, as shown in Figure 1-5, the entire world is in a critical situation with rising temperatures, decreasing sea ice extent, rising sea surface temperatures and sea levels, and tropical cyclones becoming stronger. The threat of more frequent, and more severe damage caused by heavy rainfall disasters, river flooding, landslides, or frequent storm surges is increasing.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-5%20%E6%BF%80%E7%94%9A%E5%8C%96%E3%81%99%E3%82%8B%E7%81%BD%E5%AE%B3%E3%81%AE%E4%BE%8B.png?raw=true" width="60%">
（Source）The “Future Tokyo” Strategy Vision (Summary Version) (December 2019)<br>

**Figure 1-5　Examples of increasingly severe disasters**<p>

Furthermore, as displayed in Figures 1-6 and 1-7, the risk of earthquakes such as the one directly under the Tokyo metropolitan area which is assumed to have a 70% probability of occurring in the next 30 years, and the Nankai Trough giant earthquake is also increasing.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-6%20%E9%A6%96%E9%83%BD%E7%9B%B4%E4%B8%8B%E5%9C%B0%E9%9C%87%E7%AD%89%E3%81%AB%E3%82%88%E3%82%8B%E6%9D%B1%E4%BA%AC%E3%81%AE%E8%A2%AB%E5%AE%B3%E6%83%B3%E5%AE%9A.png?raw=true" width="60%">
（Source）Estimated damage to Tokyo due to an earthquake directly under the Tokyo metropolitan area (April 2012 Publication） <br>
https://www.bousai.metro.tokyo.lg.jp/taisaku/torikumi/1000902/1000401.html<br>

**Figure 1-6　Estimated damage to Tokyo due to an earthquake directly under the Tokyo metropolitan area**<p>

 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-7%20%E5%8D%97%E6%B5%B7%E3%83%88%E3%83%A9%E3%83%95%E5%B7%A8%E5%A4%A7%E5%9C%B0%E9%9C%87%E7%AD%89%E3%81%AB%E3%82%88%E3%82%8B%E5%B3%B6%E3%81%97%E3%82%87%E3%81%AE%E8%A2%AB%E5%AE%B3%E6%83%B3%E5%AE%9A.png?raw=true" width="60%"><br>
（Source）Estimated damage to the islands due to Nankai Trough Earthquake, etc.(May 2013 Publication）<br>
https://www.bousai.metro.tokyo.lg.jp/taisaku/torikumi/1000902/1000402.html<br>
**Figure 1-7　Estimated damage to the islands due to Nankai Trough Earthquake**<p>

 
****▼Responding to changes in human flow and logistics is key to inter-city competition.****

Figure 1-8 clearly shows the number of air passengers worldwide is expected to nearly double to 7.8 billion by 2036, and if we do not meet the strong demand for international business jets and other services, we will fall behind the world.


 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-8%20%E4%B8%BB%E3%81%AA%E5%9B%BD%E3%81%AE%E8%88%AA%E7%A9%BA%E6%97%85%E5%AE%A2%E6%95%B0%E3%81%AE%E5%B0%86%E6%9D%A5%E6%8E%A8%E8%A8%88.png?raw=true" width="60%"><br>
 （Source）Based on “Vision for ‘Future Tokyo’ Strategy” (December 2019）<br>
**Figure 1-8　Estimated future air passenger traffic in major countries**


Figure 1-9 also points out that because the EC market is expected to expand further, if the infrastructure for new means of transportation such as drone delivery is delayed, we will be left behind the world.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-9%20%E6%97%A5%E6%9C%AC%E3%81%AEBtoC-EC%EF%BC%88%E9%9B%BB%E5%AD%90%E5%95%86%E5%8F%96%E5%BC%95%EF%BC%89%E5%B8%82%E5%A0%B4%E8%A6%8F%E6%A8%A1%E3%81%AE%E6%8E%A8%E7%A7%BB.png?raw=true" width="60%"> 
（Source）Ministry of Economy, Trade and Industry, "FY2019 International Economic Research Project for Building an Integrated Domestic and Foreign Economic Growth Strategy (Market Survey on Electronic Commerce) Report
https://www.meti.go.jp/press/2020/07/20200722003/20200722003.html

**図1-9　B to C-EC (electronic commerce) market size in Japan**<p>


****▼Pursuing a "new life" with the experience gained through the COVID-19 Disaster.****

The voluntary restraint on going out due to the Corona disaster restricted conventional real-life "connections." While the younger generation has still kept interacting online, many people reaffirmed the importance of "connections" between the people. It is necessary to utilize the experience gained from the Corona Disaster to weave "new connections" through a hybrid of the real and virtual, and create a society in which a new everyday life has taken root.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-10%20%E3%80%8E%E6%9C%AA%E6%9D%A5%E3%81%AE%E6%9D%B1%E4%BA%AC%E3%80%8F%E6%88%A6%E7%95%A5%E3%81%AB%E3%81%8A%E3%81%91%E3%82%8B%E3%80%8C%E6%96%B0%E3%81%97%E3%81%84%E6%9A%AE%E3%82%89%E3%81%97%E3%80%8D%E3%81%AE%E8%BF%BD%E6%B1%82.png?raw=true" width="60%">  <br>
（Source）Based on “Future Tokyo” Strategy (March 2021)<br>
**Figure 1-10　Pursuing “New Lifestyles” in the “Future Tokyo” Strategy**<p>
  
****▼Creating a strong and sustainable society that generates new value.****

In recovering from the crisis of the Corona disaster, it is necessary not simply to return to the society that existed before the Corona disaster, but to upgrade policies from the perspective of "sustainable recovery" which extends to the realization of sustainable lifestyles for people. Creation of a strong and sustainable society that creates new values while flexibly responding to changing circumstances is also required for this purpose.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-11%20%E3%80%8C%E3%82%B5%E3%82%B9%E3%83%86%E3%83%8A%E3%83%96%E3%83%AB%E3%83%BB%E3%83%AA%E3%82%AB%E3%83%90%E3%83%AA%E3%83%BC%E3%80%8D%E3%81%AE%E5%AE%9F%E7%8F%BE.png?raw=true" width="60%">  <br>
（Source）Based on “Future Tokyo” Strategy (March 2021)<br>
**Figure 1-11　Realize “Sustainable Recovery**

  
****▼As a city with diversity, it is necessary to be attentive to diverse values.****

People of various backgrounds including gender, age, nationality, and race are living in Tokyo. New human rights issues are emerging against a backdrop of diversifying values and increasingly complex social structures. Tokyo, aiming to become a truly diverse city, must be attentive to these diverse values.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-12%20%E5%A4%9A%E6%A7%98%E3%81%AA%E9%83%BD%E6%B0%91%E3%83%8B%E3%83%BC%E3%82%BA%E3%81%B8%E3%81%AE%E5%AF%BE%E5%BF%9C%EF%BC%88%E7%9B%AE%E5%BA%A7%E3%81%992040%E5%B9%B4%E4%BB%A3%E3%81%AE%E6%9D%B1%E4%BA%AC%E3%81%AE%E5%A7%BF%EF%BC%89.png?raw=true" width="60%">  <br>
（Source）Based on “Future Tokyo” Strategy (March 2021)<br>
**Figure 1-12　Responding to the diverse needs of Tokyo residents (The Tokyo of the 2040s as we aspire to be)**

  
****▼Strongly promote DX in all fields, and drastically change the industrial structure.****

The Tokyo Metropolitan Government will strongly promote DX in all fields to pioneer the "Tokyo of the Future." In order to realize this goal, it will require a major transformation of the industrial structure in a positive and digital way including changes in new services and business categories with an eye to the transformation of people's lifestyles, due to the Corona Disaster.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-13%20%E3%80%8C%E7%88%86%E9%80%9F%E3%80%8D%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E5%8C%96%E3%81%A8%E6%A7%8B%E9%80%A0%E6%94%B9%E9%9D%A9.png?raw=true" width="60%">  <br>
（Source）Based on “Future Tokyo” Strategy (March 2021)<br>
**Figure 1-13　Digitalization and structural reforms**

****▼We will promote initiatives that are comparable to those of overseas cities.****

Many developed countries make efforts to address the digital twin.

For example in Australia, the Department of Environment, Land, Water and Planning (DELWP) in the state of Victoria has released highly detailed, high-quality 3D city models covering 20 regional cities across the state as open data. The platform allows users to examine road visibility and analyze the effects of building shadows.

In Finland, a government-led project is being implemented to digitize cities against the backdrop of BIM utilization in the private sector. In Helsinki, the capital of Finland, the city is building a 3D city model, creating and publishing a viewer, and creating open data in the Kalasatama area of the city. Specifically, the city is developing a simulation platform that includes analysis functions for wind environment, amount of sunlight, building shadows, etc.

In the United Kingdom, the National Underground Asset Register (NUAR) is under developing. This system is aimed to design a mapping information infrastructure for underground infrastructure owners to securely share existing underground asset data with authorized users (telecommunications, electricity, gas, water, sewage, municipalities, etc.).

In Singapore, the Singapore Land Authority (SLA) has established One map 3D, a platform that provides geospatial information of roads and buildings, land ownership, nearest schools, and demographic data of the location/neighborhood, etc. One map 3D's function enables us to plan drone flight paths, or visualize of information such as bus stop waiting times.

In order for Tokyo to compete with other international cities, it is necessary not only to keep up with overseas efforts, but also to take the initiative in implementing new initiatives ahead of other countries.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-14%20%E6%B5%B7%E5%A4%96%E3%81%AB%E3%81%8A%E3%81%91%E3%82%8B%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AB%E9%96%A2%E9%80%A3%E3%81%97%E3%81%9F%E5%85%88%E9%80%B2%E7%9A%84%E3%81%AA%E5%8F%96%E3%82%8A%E7%B5%84%E3%81%BF.png?raw=true" width="60%">  <br>
（Source）Victoria State Government HP（ https://www.land.vic.gov.au/maps-and-spatial/maps-and-spatial-news/3d-buildings-data-of-major-victorian-regional-centres-now-available ）<br>
（Source）Kalasatama Digital Twin（ https://www.hel.fi/static/liitteet-2019/Kaupunginkanslia/Helsinki3D_Kalasatama_Digital_Twins.pdf ）<br>
（Source）Case Study: National Underground Asset Register (NUAR) Pilot Programme」（ https://www.cdbb.cam.ac.uk/news/case-study-NUAR-pilot-programme ）<br>
（Source）Singapore Land Authority（SLA）「OneMap3D」（ https://www.onemap3d.gov.sg/main/ ）<br>
**Figure 1-14　Advanced approaches related to Digital Twin overseas**

****▼As the capital of Japan, it is required to promote the spread of the project to other cities in Japan.****

In advanced municipalities (e.g. Shizuoka Prefecture), the sprouting of initiatives aimed at a digital twin, such as the development of 3D models of cities, has been confirmed. As the capital of Japan, Tokyo is also expected to play a role in promoting the spread of innovations to other cities in Japan by implementing them ahead of other cities and demonstrating their effectiveness.

****▼Tokyo, the world's most open city, attracting people, goods, and money from all over the world.****

Tokyo, as Japanese gateway, will be able to powerfully drive the Japanese economy by improving its attractiveness through digitalization and by winning the international inter-city competition.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-15%20%E4%B8%96%E7%95%8C%E4%B8%80%E3%82%AA%E3%83%BC%E3%83%97%E3%83%B3%E3%81%AA%E6%9D%B1%E4%BA%AC%EF%BC%88%E7%9B%AE%E6%8C%87%E3%81%992040%E5%B9%B4%E4%BB%A3%E3%81%AE%E6%9D%B1%E4%BA%AC%E3%81%AE%E5%A7%BF%EF%BC%89.png?raw=true" width="60%">  <br>
（Source）Based on “Future Tokyo” Strategy (March 2021)<br>
**Figure 1-15　Tokyo will be the world’s most open city (The Tokyo of the 2040s as we aspire to be**

****▼Leading Japan through the spread to other municipalities under the banner of social implementation in Tokyo.****

Based on the internal and external environment surrounding TMG, the following four points can be considered significant for TMG's Digital Twin initiative (Figure 1-16).

①Extremely complex and diverse issues are concentrated

②Necessity of a social infrastructure that contributes to solving issues and improving the quality of life of Tokyo residents

③Tokyo will be the first city to implement the Digital Twin, and by demonstrating its effectiveness, it will promote the spread of the Digital Twin to other cities in Japan.

④Potential to get a competitive advantage in international urban competition

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%201-16%20%E6%9D%B1%E4%BA%AC%E9%83%BD%E3%81%8C%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AB%E5%8F%96%E3%82%8A%E7%B5%84%E3%82%80%E6%84%8F%E7%BE%A9.png?raw=true" width="60%">  
  
**Figure 1-16　Significance of Tokyo’s Digital Twin Initiative**

The Tokyo Metropolitan Government's Digital Twin Realization Project shall aim to establish a digital twin for both internal use by the agency and standard use by the citizens of Tokyo, and by opening up APIs, access will be also allowed for external companies and organizations that wish to use the system. This project is not intended to negate existing digital twin initiatives by local governments or individual private companies. We believe that digital twins developed for different purposes and in different fields can enhance the value of each other by linking their data and systems if needed.

<a  id="anchor1.3"></a>
<a  href="#anchor1.3"></a>
### 1.3 Tokyo Metropolitan Government's Initiatives Related to Digital Twin

****▼Positioning the promotion of the digital twin in long-term strategy.****

The promotion of the digital twin has been clearly positioned in the long-term strategies formulated by the Tokyo Metropolitan Government to date.

In the "Strategic Vision for 'Future Tokyo'" released in December 2019, as a project to realize the digital twin, the Tokyo Metropolitan Government has set forth the construction of a public-private collaborative data platform after 2020 and the realization of a digital twin through the fusion of cyber space and physical space.

In addition, the "Smart Tokyo Implementation Strategy" released in February 2020, the promotion of the digital twin was identified as supporting the realization of the three types of cities (safe city, diversity city, and smart city). The expected effects of the Digital Twin are "updating the metropolitan government," "improving the quality of life of Tokyo residents and visitors," and "improving the earning power of Tokyo businesses.

In the "Future Tokyo" Strategy released in March 2021, "Strategy 10: Smart Tokyo/TOKYO Data Highway Strategy" was set forth as one of the 20+1 "strategies" to be addressed toward 2030, and it is expected that by 2030, real-time data will be available in all fields and will be used for decision-making and policy-making. The strategy calls for the "realization of a complete digital twin" where real-time data can be utilized in all fields for decision-making and policy-making by 2030. 

さらに、2022年2月公表した「『未来の東京』戦略 version up 2022」においては、デジタルツインの実現に向けた基盤整備を加速するとして、「デジタルツインの基礎となる3D地形データを都内全域で整備」「防災分野での先行的活用」「東京データプラットフォームの本格運用に向けた取組を推進」を掲げている。

<a  id="anchor2"></a>
<a  href="#anchor2"></a>
### 2. Our goal through Digital Twin

<a  id="anchor2.1"></a>
<a  href="#anchor2.1"></a>
### 2.1 Value of Digital Twin

****▼Digital Twin Improves QOL of Tokyo Residents and QOS of Tokyo Metropolitan Government.****

There are three main effects expected from the realization of the digital twin as shown in Figure 2-1.

The first is that the status of the city in physical space (real space) can be grasped in cyberspace in real time. For example, by using traffic data and human flow data obtained from sensors installed in the city, it is possible to obtain and visualize realtime-congestion status of specific roads and trains, or the "current" waiting time at various administrative counters. This will enable wheelchair users, tourists with heavy luggage to avoid crowded vehicles, and Tokyo residents to visit administrative agencies during relatively uncrowded times of the day.

Secondly, analysis and simulation using the latest, real-time data will be freely available. For example, in the field of disaster prevention, it will be possible to predict the risk of flooding in cyberspace using river cross section data from river area maps acquired in physical space and real-time measurement information on river water levels, by combining them with meteorological data, and by using the results in physical space we can make decisions on opening and closing sluice gates and flume gates. In the field of urban development, the project is expected to be used for urban planning and urban development. In the field of urban development, data from various sensors and traffic volumes installed in cities can be used to understand the state of infrastructure, and simulations of future deterioration can also be performed.

Third, by feeding back the results of visualization, analysis, and simulation to the physical space, the data can be used for various purposes. For example, in the field of disaster prevention, it is expected to provide real-time alerts to smartphones near rivers when the risk of river flooding increases. In the field of urban development, it is expected to improve operational efficiency and to formulate and evaluate plans based on data, for example, by regularly monitoring the condition of infrastructure and by simulating the state of deterioration, so that inspections can be carried out with priority on areas that are deteriorating rapidly.

Through the realization of such a digital twin, we aim to improve the QOS of the Tokyo Metropolitan Government, as well as improve the quality of life of Tokyo residents, and utilize this information in decision-making, policy-making, and other situations.

  
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%202-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%8F%90%E4%BE%9B%E4%BE%A1%E5%80%A4.png?raw=true" width="60%">  

 **Figure 2-1　Values of Digital Twin**

<a  id="anchor2.2"></a>
<a  href="#anchor2.2"></a>
### 2.2 What is the complete digital twin that we aim to realize?

****▼Based on existing plans and related policies, 9 fields are assumed as focus fields.****

In aiming to realize the Digital Twin based on the "Smart Tokyo Implementation Strategy," the nine areas of "disaster prevention, urban planning, mobility, energy, nature, wellness, education, work style, and industry" shown in Figure 2-2 were set as focus areas.

In setting the focus areas, we used the nine study areas in the "Smart Tokyo Implementation Strategy," which is a high-level plan, as a base, and compared them to the study areas, services, and fields in related plans.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%202-2%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E5%AF%BE%E8%B1%A1%E5%88%86%E9%87%8E%E3%83%BB%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9.png?raw=true" width="60%">  
 
**Figure 2-2　Digital Twin Target Areas and Services**<p>


****▼Realize the digital twin by 2030 and build a continuous improvement cycle by 2040.****

The goal of the digital twin is to be realized by 2030 and to be developed as a continuous improvement cycle by 2040.

The "complete digital twin" to be realized here is defined as "a state in which 3D city models and interfaces are maintained and continuously updated, and a variable mechanism is established in which "some" data of the city can be used for decision-making by the metropolitan government, businesses, and citizens in "all" target fields, and for policy making by the metropolitan government".

By 2030, the goal is to expand the use of the digital twin in terms of both the "government, companies, and citizens" who are the users and the fields in which they are used (the nine focus areas), and to utilize "some" data of the city in "all" target fields. In addition, about the 3D urban models and interfaces of the digital twin, a system that guarantees variability and continuous updating will be established. Furthermore, the goal by 2040 is to realize advanced simulations by utilizing diverse and highly accurate data by accumulating and passing on the obtained data.

<a  id="anchor3"></a>
<a  href="#anchor3"></a>
### 3. Components of Digital Twin

<a  id="anchor3.1"></a>
<a  href="#anchor3.1"></a>
### 3.1 Overall Picture of Digital Twin

****▼The digital twin consists of 4 elements: Strategy, Foundational Elements, Ancillary Elements, and Services****

Figure 3-1 shows the elements required to realize the digital twin. The digital twin consists of four elements: strategy, infrastructure, ancillary elements, and services. Each element is not independent of the others, but rather they influence each other. That is why it is important to consider the constraints and influences of other elements appropriately.

　The structure of the digital twin was examined by Government of Japan, by referring to the "Smart City Reference Architecture White Paper," which is a result of the "Strategic Innovation Program (SIP) Phase 2: Cyberspace Infrastructure Technology Architecture Development and Demonstration Research Project Using Big Data and AI" by the Cabinet Office.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%203-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E5%85%A8%E4%BD%93%E5%83%8F.png?raw=true" width="60%">

 **Figure 3-1　Overall Picture of Digital Twin**

<a  id="anchor3.2"></a>
<a  href="#anchor3.2"></a>
### 3.2 Components of Digital Twin

****▼Data, Systems, Infrastructure, and Security are defined as the fundamental elements of the Digital Twin.****

We have decomposed and defined the basic elements of the digital twin into three categories: cyberspace, physical space, and common. Cyber space consists of "data" to be utilized on the digital twin and "systems" that operate on the digital twin. Physical space consists of "infrastructure," which is facilities and equipment for generating and transmitting digital data to be utilized on the digital twin. In addition, "security" is an element that should be provided in both cyber and physical space, and is a necessary function to protect the digital twin from internal and external threats. On Table 3-1, the components of the digital twin are listed.

 **Table 3-1 Components of Digital Twin**

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%A7%8B%E6%88%90%E8%A6%81%E7%B4%A0.png?raw=true" width="60%">

<a  id="anchor3.3"></a>
<a  href="#anchor3.3"></a>
### 3.3 Components of Cyber Space

****▼Data and Systems are defined as components of Cyber Space.****

Cyberspace shall consist of "data" and "systems". The data consists of "data" used for analysis and simulation on the digital twin. Systems consist of "applications" for simulations on the digital twin, "databases" as an environment for storing various data utilized on the digital twin, and "interfaces" for linking with data and systems. Table 3-2 shows the components of cyberspace, and Table 3-3 shows examples of data types handled by the digital twin.

 **Table 3-2 Components of Cyberspace**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-2%20%E3%82%B5%E3%82%A4%E3%83%90%E3%83%BC%E7%A9%BA%E9%96%93%E3%81%AE%E6%A7%8B%E6%88%90%E8%A6%81%E7%B4%A0.png?raw=true" width="60%">

 **Table 3-3 Example of data**

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-3%20%E3%83%87%E3%83%BC%E3%82%BF%E3%81%AE%E4%BE%8B.png?raw=true" width="60%">
 
<a  id="anchor3.4"></a>
<a  href="#anchor3.4"></a>
### 3.4 Components of Physical Space

****▼Infrastructure is defined as components of physical space.****

The infrastructure that constitutes the physical space consists of "sensing devices" for data conversion and "networks" for linking them, with the objective of generating the data necessary to conduct analysis and simulation on the digital twin. Table 3-4 displays the components of the physical space.

 **Table 3-4 フComponents of Physical Space**

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-4%20%E3%83%95%E3%82%A3%E3%82%B8%E3%82%AB%E3%83%AB%E7%A9%BA%E9%96%93%E3%81%AE%E6%A7%8B%E6%88%90%E8%A6%81%E7%B4%A0.png?raw=true" width="60%">

<a  id="anchor3.5"></a>
<a  href="#anchor3.5"></a>
### 3.5 Elements common to Cyber and Physical Space

****▼Security is defined as a common element of Cyber and Physical Space.****

Security refers to the functions and matters needed to protect the digital twin from internal and external threats. There are two types of security measures for a digital twin: those that the components of the digital twin should be equipped with (technical measures) and those that are necessary for operating and managing the digital twin (administrative measures). Table 3-5 shows the requirements of each.

 **Table 3-5 Security Requirements**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-5%20%E3%82%BB%E3%82%AD%E3%83%A5%E3%83%AA%E3%83%86%E3%82%A3%E3%81%AE%E8%A6%81%E4%BB%B6.png?raw=true" width="60%"> 

<a  id="anchor3.6"></a>
<a  href="#anchor3.6"></a>
### 3.6 Other Factors

****▼Present elements and ideas on Strategy, Ancillary Elements, and Services.****

In realizing the digital twin, it is also necessary to consider three elements: "strategy," which serves as a guideline for designing the digital twin, "ancillary elements" related to operations, and "services." The concepts of these elements are shown in Table 3-6.

 **Table 3-6 Other Factors**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-6%20%E3%81%9D%E3%81%AE%E4%BB%96%E3%81%AE%E8%A6%81%E7%B4%A0.png?raw=true" width="60%"> 

****▼Digital twin scales are categorized as Building, Area, and City.****

As shown in Table 3-7, digital twins can be classified into three scales: "building," "area" which is a collection of multiple buildings, and "city" which is a collection of buildings and areas. Digital twins at each scale have different operating entities and operational objectives. At first, the TMG will start the development and operation of the urban digital twin, but in the future, the TMG will also work to interoperate data and functions at each scale in order to enhance the value of the digital twin.

 **Table 3-7 Digital Twin Scale**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-7%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E3%82%B9%E3%82%B1%E3%83%BC%E3%83%AB.png?raw=true" width="60%"> 

About the urban digital twin developed and operated by the Tokyo Metropolitan Government, Figure 3-2 shows an operational model, Table 3-8 shows examples of each entity in the operational model, and Table 3-9 shows examples of the roles of each entity. The digital twin shall be operated by data providers, operators, agency users, and service providers and users mutually linking their data. In addition to this, an external evaluation should be conducted by advisors and evaluators to assess whether the digital twin is operating appropriately.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%203-2%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E9%81%8B%E7%94%A8%E3%83%A2%E3%83%87%E3%83%AB.png?raw=true" width="60%">

 **Figure 3-2 Operational model of Digital Twin**

 **Table 3-8 Entities of Digital Twin (Example)**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-8%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E4%B8%BB%E4%BD%93%EF%BC%88%E4%BE%8B%EF%BC%89.png?raw=true" width="60%"> 

 **Table 3-9 Roles of entities (Example)**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-9%20%E5%90%84%E4%B8%BB%E4%BD%93%E3%81%AE%E5%BD%B9%E5%89%B2%EF%BC%88%E4%BE%8B%EF%BC%89.png?raw=true" width="60%"> 

****▼Examples of items to consider regarding rules and specifications were defined.****

In developing and operating a digital twin and providing various measures and services, it is important to comply with relevant laws and regulations set by the government. Setting appropriate rules for the entities operating the digital twin and related entities, and considering standard specifications to promote mutual use are also needed for this purpose. Examples of items to be considered in the development and operation of the digital twin are listed below in Table 3-10.

 **Table 3-10 Items to consider for digital twin rules and specifications (Example)**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%203-10%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E3%83%AB%E3%83%BC%E3%83%AB%E3%83%BB%E4%BB%95%E6%A7%98%E3%81%AE%E6%A4%9C%E8%A8%8E%E4%BA%8B%E9%A0%85%EF%BC%88%E4%BE%8B%EF%BC%89.png?raw=true" width="60%"> 

<a  id="anchor4"></a>
<a  href="#anchor4"></a>
### 4. Steps toward realizing Digital Twin

<a  id="anchor4.1"></a>
<a  href="#anchor4.1"></a>
### 4.1 Steps to realize Digital Twin

****▼Supposing three phases to realize the Digital Twin.****

As indicated in Section 2.2, the goal is to realize the digital twin by 2030 and to develop it into a continuous improvement cycle by 2040. As shown in Figure 4-1, the following three phases will be set up for the realization of the digital twin: "Establishment of digital twin infrastructure" phase (Phase 1) starting in FY2020, "Expansion of digital twin operation and use" phase (Phase 2) starting in FY2023, and "Full realization and advancement of the digital twin" phase (Phase 3) starting in FY2030. Phase 3 is the "realization and advancement of a complete digital twin" phase, which will begin in FY2030 and thereafter. This roadmap focuses on implementation items for Phase 1, which is the scope for the time being.
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E5%AE%9F%E7%8F%BE%E3%81%AB%E5%90%91%E3%81%91%E3%81%9F%E3%83%95%E3%82%A7%E3%83%BC%E3%82%BA.png?raw=true" width="60%">

**Figure 4-1 Three phases to realizes Digital Twin**

****▼For the time being, construction of platform and ecosystem, rule development, and implementation of services in priority fields are focused.****

To realize the Digital Twin, in Phase 1, which is the phase to build the infrastructure for the Digital Twin, the first step is to establish the Digital Twin infrastructure and data ecosystem so that the Digital Twin can be used in the Agency's internal operations. In this phase, we will initially study and develop the specifications and rules for the construction, operation, and maintenance of the digital twin infrastructure and data ecosystem, and implement use cases and beta version projects for service implementation.

In Phase 2, which is the phase to work on the operation, expansion of use, and external collaboration after the establishment of the infrastructure, the following issues will be considered for the implementation of services in priority fields: examination of the mechanism for data linkage and updating within and outside the agency, development and functional expansion of simulators necessary for analysis and simulation, and the addition of specifications and rules based on actual operation and trends in the government and other countries. In addition to adding and updating specifications and rules based on actual operations and trends in the government and other countries, we will begin to study specifications and rules for the use of real-time data in anticipation of Phase 3. 

In Phase 3, the systems, infrastructure, specifications and rules necessary to handle more real-time data and services will be studied and developed.

The strategies required in each phase shall be examined and updated, reflecting the opinions of experts at the study group. Figure 4-2 shows the steps toward the realization of the digital twin. The items to be implemented in each phase shall be reviewed and updated whenever there is a decision or change in the policy.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-2%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E5%AE%9F%E7%8F%BE%E3%82%B9%E3%83%86%E3%83%83%E3%83%97.png?raw=true" width="60%">
 
**Figure 4-2 Steps to realize Digital Twin**

<a  id="anchor4.2"></a>
<a  href="#anchor4.2"></a>
### 4.2 Implementation of base elements

****▼The Digital Twin Platform is established to serve as a node for data linkage in order to aggregate and utilize data in TMG.****

Since the Digital Twin is operated by linking data from each entity to each other, a secure environment is required to consolidate data from both inside and outside the Agency and to provide services that utilize such data. Therefore, a "digital twin infrastructure" consisting of an "Agency Data Store" that aggregates and stores data from both internal and external entities, a "Data Catalog" and "Interface" for referencing and using each data, and a "Viewer" for visualizing the data, should be constructed. The positioning of the digital twin infrastructure in the data flow is shown below (Figure 4-3). The digital twin infrastructure will be used as a nodal point to link each type of data.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-3%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E3%83%87%E3%83%BC%E3%82%BF%E3%83%95%E3%83%AD%E3%83%BC%E3%81%AB%E3%81%8A%E3%81%91%E3%82%8B%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E5%9F%BA%E7%9B%A4%E3%81%AE%E4%BD%8D%E7%BD%AE%E3%81%A5%E3%81%91.png?raw=true" width="60%">
 
**Figure 4-3 Position of the digital twin platform in the data flow**

Data, systems, and infrastructure need to be developed in accordance with the services to be realized. Each element is distinguished into two categories as shown in Figure 4-4: those to be commonly maintained in all fields, and those to be maintained after considering requirements and specifications according to the services to be realized in each field. At the start of Digital Twin operation (at the completion of Phase 1), viewers, databases, a part of geospatial data, and a part of static data shall be developed, and the remaining elements shall be developed and completed in stages. 

As for the data, the Agency has begun consolidating its data and releasing it to viewers outside the Agency from FY2021(Table 4-1).

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-4%20%E6%95%B4%E5%82%99%E5%8C%BA%E5%88%86%E3%81%AE%E3%82%A4%E3%83%A1%E3%83%BC%E3%82%B8.png?raw=true" width="60%">
 
**Figure 4-4 Image of Development Category**

 **Table 4-1 Examples of Internal Data being aggregated and provided**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-1%20%E9%9B%86%E7%B4%84%E3%83%BB%E6%8F%90%E4%BE%9B%E3%82%92%E8%A1%8C%E3%81%A3%E3%81%A6%E3%81%84%E3%82%8B%E5%BA%81%E5%86%85%E3%83%87%E3%83%BC%E3%82%BF%E4%BE%8B.png?raw=true" width="60%"> 
 
<a  id="anchor4.3"></a>
<a  href="#anchor4.3"></a>
### 4.3 Maintenance of ancillary elements

****▼Continuing considering legal actions or studies to be taken by TMG.****

There are various legal and institutional issues involved in the development and operation of the digital twin. For example, when acquiring data and constructing a digital twin, there are issues related to "people," such as portrait and privacy rights when acquiring video data and personal information protection when acquiring location information, as well as "cities," such as the reflection of architectural and artistic works that are considered copyrightable. In addition, there is the viewpoint of whether the reproduction of real space in the construction of a digital twin will be regarded as a reproduction or adaptation of a copyrighted work, or an infringement of the right to preserve the identity of a work. In addition, it is necessary to consider whether the acquired data can be processed when analyzing the data, and whether institutional issues can be cleared when providing services and releasing data.

In the future, the Tokyo Metropolitan Government will consider its response to the realization of the digital twin based on the status of studies by the national government and related organizations after identifying the issues to be discussed.

  
**Table 4-2 Examples of Tokyo Metropolitan Government's implementation matters regarding legal system**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-2%20%E6%B3%95%E5%88%B6%E5%BA%A6%E9%9D%A2%E3%81%AB%E9%96%A2%E3%81%99%E3%82%8B%E6%9D%B1%E4%BA%AC%E9%83%BD%E3%81%AE%E5%AE%9F%E6%96%BD%E4%BA%8B%E9%A0%85%E3%81%AE.png?raw=true" width="60%"> 

****▼Organizing rules and guidelines for Digital Twin operation and internal data provision on a priority basis.****

In the development and operation of the digital twin, various rules and guidelines are needed to ensure more efficiency. To operate the digital twin, the priority is to examine and develop rules and guidelines for the operation of the infrastructure and the handling of data within the government agencies.

Regarding the "basic policy for the operation of the infrastructure," it is necessary to consider the policy for the operation and the procedures for its use.

Regarding internal data, we have to consider data maintenance, data provision, and data use. Regarding "data development within the Agency," especially about data acquisition, it is necessary to consider arrangements for the use of generated and acquired data in each project on the digital twin, as well as the open data licensing policy when acquiring data for the purpose of public disclosure. About "data provision," considering procedures and rules for providing data to the Digital Twin Agency Infrastructure is needed. As for "data use," it is necessary to consider licenses for using data on the digital twin both within and outside the government, and terms of use such as whether data processing is allowed or not. For data use, it is also required to consider rules for supporting users' data cleansing and the method-and -format of feedback by users to the data and infrastructure.

 **Table 4-3 Examples of implementations related to terms and guidelines**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-3%20%E8%A6%8F%E7%B4%84%E3%83%BB%E3%82%AC%E3%82%A4%E3%83%89%E3%83%A9%E3%82%A4%E3%83%B3%E3%81%AB%E9%96%A2%E3%81%99%E3%82%8B%E5%AE%9F%E6%96%BD%E4%BA%8B%E9%A0%85%E3%81%AE%E4%BE%8B.png?raw=true" width="60%"> 
 
The license of open data defines the conditions under which it can be used, modified, redistributed, sold, and so on.

The CC (Creative Commons) license is a general copyright license. There are various classifications of licenses, for example CC, which is a general copyright license, ODC (Open Data Commons), which is a license for data/databases, and PD (Public Domain), which is a license that does not belong to anyone.

As of February 28, 2022, the CC license is used in the government's Standard Terms of Use and the metropolitan government's open data license, but the CC license has some restrictions, such as strict limitations on the use of Digital Rights Management (DRM). However, the CC license has severe restrictions on the use of DRM and other limitations.

In the development of open data, it is necessary for each data development entity to consider licensing in light of the above.

****▼Formulation of data standards, data quality, tools, and operation rules is important for cross-organizational data collaboration.****

On the operation of the digital twin, it is important for each entity to coordinate data across the board. Various organizations within and outside the government will be involved in the operation of the digital twin, but in case that each organization maintains and manages data based on its own individual specifications and rules, data utilization and coordination will be limited. To operate the digital twin efficiently and effectively through cross-organizational data coordination, it is important to create an environment that enables efficient data utilization and coordination across all entities involved in the digital twin operation. Therefore, for the time being "data standards," "data quality," "tools," and "operation rules" for data utilization will be developed with reference to the specifications and approaches of the government and related organizations(Table 4-4). Examples of guidelines related to the standard specifications are shown in Table 4-5.

 **Table 4-4 Examples of implementation related to standard specification**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-4%20%E6%A8%99%E6%BA%96%E4%BB%95%E6%A7%98%E3%81%AB%E9%96%A2%E3%81%99%E3%82%8B%E5%AE%9F%E6%96%BD%E4%BA%8B%E9%A0%85%E3%81%AE%E4%BE%8B.png?raw=true" width="60%"> 
 
**Table 4-5 Examples of documents related to standard**

  <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-5%20%E6%A8%99%E6%BA%96%E4%BB%95%E6%A7%98%E3%81%AB%E9%96%A2%E3%81%99%E3%82%8B%E3%83%89%E3%82%AD%E3%83%A5%E3%83%A1%E3%83%B3%E3%83%88%E3%81%AE%E4%BE%8B.png?raw=true" width="60%"> 
 
<a  id="anchor4.4"></a>
<a  href="#anchor4.4"></a>
### 4.4 Service Implementation

****▼Implementing services in 9 priority fields based on beta projects and other factors****

Future Digital Twin services will be implemented and utilized in 9 fields, based on the use cases of Digital Twin considered by each bureau, the results of demonstrations such as beta projects, and the efforts of private companies.

In each field, the following services are envisioned as examples. The services listed below are only examples, and are not limited to those planned for service implementation. The contents of the services will be revised as necessary as the plans and related policies of each field and the use cases of the digital twin for each field are discussed with the bureaus and private operators.

(1)	Examples of Disaster Prevention Field Services

****▼Disaster Simulation****

　By simulating disasters in a virtual space and predicting and analyzing the damage, the system will be used to formulate safe and secure urban development plans and evacuation plans.

****▼Real-time monitoring and abnormality detection of structures****

Monitoring and forecasting of data on flow rate, flow direction, and water pressure of drainage pipes, to detect abnormalities such as leakage and backflow at an early stage and utilize the data for prevention of flooding and inundation, review of inspection work (increase in frequency of daily inspection, etc.).

****▼Simulation of the scope of impact of a disaster****

By observing the height structure of the ground surface using satellite images, areas that will be affected by disasters like torrential rains and volcanic eruptions will be predicted and signs will be detected, which will be used to formulate safe and secure urban development plans and evacuation plans, as well as to disseminate information.

(2)	Examples of Town Planning Field Services

****▼Urban Congestion Forecasting****

Data on indoor and outdoor spaces in Tokyo (public spaces, metropolitan facilities, underground spaces, etc.) will be acquired to monitor and forecast congestion and used to disseminate congestion information to Tokyo residents and improve daily operational operations.

****▼Urban Development Simulation****

Setting hypothetical conditions for urban regeneration, urban development, landscaping, and other future visions of the city, and simulating sunlight, wind direction. This information will be utilized in development plans and explanations to the citizens of the city.

****▼Smart planning****

Utilizing data on human flow, person trips, and other data related to movement, and simulating of optimal facility layout, traffic measures, and redistribution of space such as roads in order to predict the effects of implementing each measure. These results are also used in the formulation, evaluation, and review of urban planning.

(3)	Examples of Mobility Field Services

****▼Urban traffic congestion forecasting****

The system acquires information of public transportation operations and traffic congestion in Tokyo, as well as on the availability of parking spaces at Tokyo facilities and grasps and predicts congestion conditions for use in disseminating congestion information to Tokyo residents, improving operation operations, and studying measures to relieve traffic congestion.

****▼Simulation of traffic network opening****

Establishing hypothetical conditions such as traffic volume when a new transportation network is opened, and simulating traffic volume and congestion occurrence. Then the simulation results will be used in the transportation network development plan.

****▼Automated driving simulation****

For routes where automobiles, drones, flying cars, and other vehicles are expected to operate automatically, setting up weather conditions and other hypothetical conditions, conducting operational simulations, and use the simulations to examine routes for each type of mobility.

(4)	Examples of Energy Sector Services

****▼Simulation of urban CO₂ emissions****

Toward the realization of a "Zero Emission Tokyo" that contributes to virtually zero CO₂ emissions, various urban data will be used to understand and forecast CO₂ emissions from urban activities. These results will be used to study and implement various measures to reduce emissions.

****▼Estimation of solar power generation potential****

Estimating the potential for solar power generation on roofs and walls of building facilities in Tokyo and analyzing the effects of reducing environmental impact through the use of re-energy. Then using the results to examine decarbonization measures.

****▼Simulation of optimal placement of charging facilities for ZEVs****

To promote the introduction and spread of Zero Emission Vehicles (ZEVs), simulate the optimal placement of charging facilities through traffic simulation, and use it to study the placement plan of charging facilities.

(5)	Examples of Natural Field Services

****▼Behavioral change by displaying the state of the biological and natural environment****

The carbon sink of forests, the status of climate change such as ocean acidification, and changes in ecosystems will be monitored, and how the ecological environment changes as a result of changes in the natural environment will be analyzed and used for measures to protect the biological and natural environment of Tokyo residents.

****▼VR/AR-based natural environment experience service****

Realizing XR (VR and AR) tourism experiences that reproduce the images, sounds, smells, and winds of forests, lakes, parks, etc., to improve quality of life and promote awareness of environmental conservation behaviors.

****▼Projections of climate change****

Utilizing past meteorological data, various urban data, the system predicts and displays climate change, the extent of guerrilla downpours, and the extent of impact at the time of eruptions such as Mt. Fuji.

(6)	Examples of Wellness Field Services

****▼Real-time understanding of the health behavior of Tokyo residents and action guidance****

By grasping the health behavior status of Tokyo residents through devices and cameras, and visualizing health behavior indices, health promotion measures will be implemented, and Tokyo residents will be guided to take healthier actions, contributing to an increase in healthy life expectancy.

****▼Capture and map accessibility concerns****

Hazardous areas of concern for barrier-free access will be visualized and analyzed on a 3D map, and feedback will be provided for community planning.

****▼Simulation of infectious disease prevention and control****

The data on indoor/outdoor human movement and stay will be used to study countermeasures against infectious diseases by detecting and predicting the “Three Cs” (closed spaces, crowded places and close-contact settings).

(7)	Examples of Education Field Services

****▼Experiential Education with XR****

To realize hands-on, practical education using XR (VR and AR) technology and contribute to improving the effectiveness and quality of education.

****▼Social Studies Learning with Virtual Archives of Cities****

By recording the city's history and the past of local cultural assets in a virtual space, XR technology can be used as an experiential history teaching tool for fieldwork and contribute to a better understanding of the region.

****▼Urban data acquisition study****

As part of school classes, through efforts to acquire 3D data of cities through fieldwork and integrate them into a digital twin, this service will promote understanding of the region and digital technology while acquiring data for updating 3D maps.

(8)	Examples of services in the field of working style

****▼Implementation of remote construction meetings****

Conducting construction discussions via remote meetings using underground 3D models will significantly reduce the time required for travel and status checks, contributing to the creation of extra time.

****▼Improving customer service by analyzing chat-bot text data****　

Linking an automatic response service AI chat-bot with the Digital Twin to visualize the content of inquiries by region and collect, integrate, and analyze data such as the text of inquiries to realize prioritized provision of services with high needs.

****▼VR training and seminars****

Contributing to the efficiency of seminars, training for employees and students by providing training simulators that utilize XR technology.

(9)	(9)	Examples of Industrial Field Services

****▼Digital Twin in the Manufacturing Industry****

By developing a foundation for the introduction of digital twin, which can be used in the manufacturing field of the manufacturing industry, each company will be able to introduce digital twin to enhance the sophistication and productivity of the company's production process.

****▼Promoting Digitalization of Agriculture****
To improve labor productivity in agriculture by introducing a digital twin to the agricultural production process to increase efficiency and sophistication of production.

****▼Development of virtual events****

Developing virtual events in cyberspace where various people can participate from remote locations in Japan and abroad and contributing to the activation of the event.

<a  id="anchor4.5"></a>
<a  href="#anchor4.5"></a>
### 4.5 Digital Twin area development

****▼Start developing in the Smart Tokyo prior implementation areas, and expand initiatives to other areas in Tokyo.****

As explained in 2.2, the Digital Twin will be realized by 2030 by focusing on 9 areas, and a continuous improvement cycle will be developed by 2040. However, instead of uniform development in all areas, it is desirable to limit the development to areas in each field, and develop the cycle in each area after establishing a leading model. Therefore, as shown in Figure 4-5, the policy for area development of the Digital Twin is to start with the five areas selected as leading implementation areas in the "Smart Tokyo Implementation Strategy," build a model that takes advantage of the characteristics of each area, and then aim to expand the efforts toward other areas in Tokyo. This will enable the development of enhanced data and systems which can be expected to be used in various services and use cases.

Table 4-6 displays the areas selected in the "Smart Tokyo Implementation Strategy" for prior implementation for the realization of Smart Tokyo.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-5%20%E3%82%A8%E3%83%AA%E3%82%A2%E5%B1%95%E9%96%8B%E3%82%A4%E3%83%A1%E3%83%BC%E3%82%B8.png?raw=true" width="60%">
 
**Figure 4-5 Image of are development**

**Table 4-6 Preliminary implementation areas for Smart Tokyo Realization**

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-6%20%E3%82%B9%E3%83%9E%E3%83%BC%E3%83%88%E6%9D%B1%E4%BA%AC%E5%AE%9F%E7%8F%BE%E3%81%AB%E5%90%91%E3%81%91%E3%81%9F%E5%85%88%E8%A1%8C%E5%AE%9F%E6%96%BD%E3%82%A8%E3%83%AA%E3%82%A2.png?raw=true" width="60%"> 
 
****▼In selection of the area, the regional characteristics of Tokyo and the location strategy, etc. are considered.****

The areas where initiatives will be expanded to each region of Tokyo are classified into the four categories defined in the "Grand Design for Urban Development," namely, "Central Reginal Hub Area," "New Urban Life Creation Area," "Tama Regional Hub Area," and "Natural Environment Symbiosis Area," taking into consideration the regional characteristics of Tokyo and the strategy of the centers. As shown in Figure 4-6, based on these four categories, we aim to expand from the areas where Smart Tokyo is implemented first to each cluster of centers with a view to creating new value through the formation and development of centers that utilize the individuality and potential of the region, based on the future vision of urban development. Table 4-7 shows the strategies for each of the hubs referred to when defining the area classifications.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%204-6%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%A8%AA%E5%B1%95%E9%96%8B%E3%82%A4%E3%83%A1%E3%83%BC%E3%82%B8.png?raw=true" width="60%">
 
**Figure 4-6 Image of horizontal development of Digital Twin**

**Table 4-7 Location strategy**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%204-7%20%E6%8B%A0%E7%82%B9%E6%88%A6%E7%95%A5.png?raw=true" width="60%"> 
 

****▼Develop the project from the leading areas with an eye on the regional classification of the "Grand Design for Urban Development".****

In each field, the priority areas where simulations will be conducted ahead of time will be determined based on the affinity between the field and the regional characteristics of the priority area, with taking into account existing plans and related policies. In light of the increasing frequency and severity of natural disasters in recent years or the heightened risk of earthquakes directly below the Tokyo metropolitan area, simulations will be conducted in all areas with the assumption that they will be utilized in the disaster prevention field at first. For other areas, use cases and medium- to long-term plans for digital twinning will be discussed with each bureau and organized in the second and subsequent editions of the roadmap.

<a  id="anchor5"></a>
<a  href="#anchor5"></a>
### 5. Maintenance and operation of Digital Twin

<a  id="anchor5.1"></a>
<a  href="#anchor5.1"></a>
### 5.1 Role and cost-sharing approach

Since the digital twin is expected to play a role as a future social infrastructure, it is desirable that industry, academia, and government work together to realize the digital twin. The digital twin will be established through the development and operation of each of the elements listed in section 3. Therefore, it is necessary to consider the maintenance, operation, and cost sharing with a variety of private entities. Specifically, it is expected for the government to take responsibility for the initial development and operation of data, systems, and infrastructure in fields that are highly public in terms of life and physical safety and in fields that require a long-term perspective in terms of utilization. On the other hand, for data and infrastructure that are difficult for the Tokyo Metropolitan Government to develop on its own, or for data-updates during operation, it is desirable to develop and operate them in cooperation with private companies, research institutions, and other entities outside the government with a shared responsibility.

Regarding the cost burden, it is basic that the entity responsible for the development and operation of each element bears the initial cost and the maintenance and management cost. In addition, it is desirable for the public and private entities involved in the service to share the maintenance, operation, and costs when further expansion from the elements currently in place, such as improvement of data accuracy, becomes necessary in the realization of services that utilize the digital twin.

<a  id="anchor5.2"></a>
<a  href="#anchor5.2"></a>
### 5.2 Division of roles in the development of Digital Twin

As shown in Figure 5-1, the maintenance and operation of data, systems, and infrastructure, which are the basic elements of the Digital Twin, will be shared between the TMG and entities outside the Agency. Note that "security" will be shared by each entity in charge of maintenance and operation of data, systems, and infrastructure based on the security requirements shown in 3.5. The "strategy" that defines the components of the digital twin, and the "rules and systems" and "service models" that serve as ancillary elements will be studied under the initiative of the Tokyo Metropolitan Government.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%205-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%95%B4%E5%82%99%E3%81%AB%E3%81%82%E3%81%9F%E3%81%A3%E3%81%A6%E3%81%AE%E5%BD%B9%E5%89%B2%E5%88%86%E6%8B%85.png?raw=true" width="60%">
 
**Figure 5-1 Division of roles in the development of Digital Twin**

<a  id="anchor5.3"></a>
<a  href="#anchor5.3"></a>
### 5.3 Division of roles in the operation of Digital Twin

As shown in Figure 5-2, the Digital Twin will be operated in an integrated manner, and each role are shared by both internal and external entities in accordance with the policy set by the infrastructure operator.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%205-2%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E9%81%8B%E7%94%A8%E3%83%95%E3%83%AD%E3%83%BC.png?raw=true" width="60%">
 
**Figure 5-2 Operation flow of Digital Twin**

In the operation of the Digital Twin, data coordination among data providers, operators, agency users, service providers, and users, i.e., provision of data and feedback, is important. For this reason, data providers such as the Tokyo Metropolitan Government's bureaus, digital twin operators, internal users, and service providers are positioned as the main entities involved in data providing and data coordination, and the construction of a data ecosystem through coordination among these entities.

****▼Data ecosystems are built by linking data among various entities.****

The data ecosystem concept is illustrated in Figure 5-3. The data provider is responsible for the maintenance of data in accordance with the specifications and quality standards set by the infrastructure operator, and for setting the licensing and usage rules for the data. Then the data is stored in the digital twin infrastructure based on the rules. The operator has a responsibility of checking the metadata format of the provided data and providing feedback to the data provider, as well as visualizing the data on the viewer. Data users such as agency users and service providers shall download the provided data in accordance with the license and terms of use, perform data cleansing according to the intended use, and provide feedback to the data infrastructure from the user's perspective.

Specific details of the operation rules will be reviewed and updated based on the knowledge and issues obtained through the construction of the infrastructure and various projects in the future.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%205-3%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E3%83%87%E3%83%BC%E3%82%BF%E3%82%A8%E3%82%B3%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0.png?raw=true" width="60%">
 
**Figure 5-3 Data Ecosystem of Digital Twin**

<a  id="anchor6"></a>
<a  href="#anchor6"></a>
### 6. Cost-effectiveness of Digital Twin Development

<a  id="anchor6.1"></a>
<a  href="#anchor6.1"></a>
### 6.1 Approach to Estimating cost

****▼Costs are estimated based on a combination of details and scope of development in each fields.****

As shown in Figure 6-1, the cost of developing the digital twin will be estimated by defining the scope and content of the data, systems, and infrastructure that make up the digital twin, based on the digital twin measures and use cases in the nine fields. In the estimation, the target areas of services and the timing of service-in for each field should be taken into account, and if technological progress is expected in the future, the possibility of future cost reduction shall also be mentioned, after clearly stating that this estimation is based on the current level of technology.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-1%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%95%B4%E5%82%99%E8%B2%BB%E7%94%A8%E3%81%AE%E8%A9%A6%E7%AE%97%E3%82%A4%E3%83%A1%E3%83%BC%E3%82%B8.png?raw=true" width="60%">
 
**Figure 6-1 Image of estimating cost of Digital Twin Development**

****▼Cost items are estimated for each element regarding the point in time when costs are incurred.****

As listed in Table 6-1, cost items and the point in time when costs are incurred for each infrastructure element should be organized to set cost items of digital twin development. About the cost items, after listing the items to be developed in the use case, the costs that will be incurred in a single year, such as the first year of development, should be categorized as initial costs, and ongoing costs should be categorized as maintenance and management costs, with focusing on the point in time when the costs are incurred. Figure 6-2 shows that initial costs and maintenance/management costs are divided into two categories when making estimates. In cases where the costs to be incurred each year are expected to differ, the costs within the period subject to estimation should be separately organized by year.

 
**Table 6-1 Example of cost items setup**
 
 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%206-1%20%E8%B2%BB%E7%94%A8%E9%A0%85%E7%9B%AE%E3%81%AE%E8%A8%AD%E5%AE%9A%E4%BE%8B.png?raw=true" width="60%"> <br>
*This is an example of maintenance for the purpose of illustrating the cost-effectiveness estimation method and does not assume a specific use case. The items to be estimated vary depending on the field and use case.<br>

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-2%20%E8%B2%BB%E7%94%A8%E3%81%AE%E8%A9%A6%E7%AE%97%E4%BE%8B.png?raw=true" width="60%"><br>
 *When costs and benefits are recorded as a monetary value at the time of development, it is necessary to convert the costs to a present value (discounted future costs and effects using the social discount rate).<br>
**Figure 6-2 Example of cost estimation**

<a  id="anchor6.2"></a>
<a  href="#anchor6.2"></a>
### 6.2 Approach to Estimating Effectiveness

****▼A framework for estimating the effects of the Digital Twin was prepared, and the development effects were estimated for use cases in each field.****

The effects of the digital twin development will be estimated as monetary values by accumulating the effects obtained from the use cases in each field. A framework that defines the effect items of Tokyo's digital twin will be prepared in advance, and the effects obtained from the specific use cases will be applied to the framework for trial calculations. In preparing the framework, we will refer to the concept of effect items set in overseas digital twin policies, while ensuring consistency with the digital twin objectives of Tokyo's higher-level policies (e.g. "Future Tokyo" strategy).

For example, the "Digital Twin Toolkit: Developing the business case for your digital twin," a document on digital twin promotion published in February 2021 by the Centre for Digital Built Britain (CDBB: a UK government-funded organization in collaboration with Cambridge University), is a reference for the digital twin promotion. In this document, quantitative estimation of the value for money of digital twin development is an essential step to justify the investment. The following five items are used to evaluate the value of the digital twin.

・	Nature – Environmental impact, Use of resources

・	Society – Impact on citizens and community

・	Human – Effects on safety, security, and work

・	Production – Impact on manufacturing and productivity

・	Finance – Investment costs, Operating costs, Revenue

Figure 6-3 shows the items and proposed estimation method (i.e. proposed framework for effect estimation) for estimating the effect of the digital twin development, with reference to the above five items and consideration of the consistency with Tokyo's top-level measures such as decarbonization, disaster prevention, and productivity improvement, as well as the purpose of Tokyo's digital twin ("improving the quality of life of Tokyo residents" and "improving the QOS of Tokyo's administration"). Figure 6-4 shows the proposed items and estimation method (i.e. proposed framework for effect estimation). This framework will be revised if needed during the discussion about use cases of the digital twin with each bureau and field.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-3%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%95%B4%E5%82%99%E5%8A%B9%E6%9E%9C%E3%81%AE%E8%A9%A6%E7%AE%97%E3%81%AE%E6%9E%A0%E7%B5%84%E3%81%BF.png?raw=true" width="60%">
 
**Figure 6-3 Framework for estimating the effects of Digital Twin Development**

We will set up digital twin services in each field and categorize each effect item into the five items mentioned above to estimate the effect of the development(Figure 6-4).

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-4%20%E3%83%87%E3%82%B8%E3%82%BF%E3%83%AB%E3%83%84%E3%82%A4%E3%83%B3%E3%81%AE%E6%95%B4%E5%82%99%E5%8A%B9%E6%9E%9C%E3%81%AE%E8%A9%A6%E7%AE%97.png?raw=true" width="60%">
 
**Figure 6-4 Estimation of the effect of Digital Twin Development**

****▼The estimation method is organized by categorizing the effect items by the target of the effect, focusing on the indicators to which the effect is attributed.****

As shown in Table 6-2, about the setting of effect items for the development of the digital twin, after organizing effect items for each target of the effect expressed in the use case, the trial calculation method should be organized by focusing on the indicators to which the effect is attributed. If multiple effect items can be set for the same use case, each effect item should have its own indicator. To avoid duplication of effects, we have to care that there is no overlap between effect items.

**Table 6-2 Example of effect item setup**
 
<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8%206-2%20%E5%8A%B9%E6%9E%9C%E9%A0%85%E7%9B%AE%E3%81%AE%E8%A8%AD%E5%AE%9A%E4%BE%8B.png?raw=true" width="60%"> <br>
*The effects that occur in the event of a disaster are organized separately from the constant effects.<br>
**This table is organized using one use case in the field of disaster prevention as an example. The items vary depending on the field or use case to be estimated.<br>

On estimating, each effect item should be calculated separately as illustrated in Figure 6-5. If adding up the effects, it is necessary to take care to add up only those items which show the effects at same time.

<img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-5%20%E5%8A%B9%E6%9E%9C%E3%81%AE%E8%A9%A6%E7%AE%97%E4%BE%8B.png?raw=true" width="60%"><br>
 *The information is based on an example use case in the field of disaster prevention for the purpose of explaining the method of estimating cost-effectiveness. The contents may differ from those of actual use cases to be considered and implemented.<br>
**Figure 6-5 Example of effect estimation**

<a  id="anchor6.3"></a>
<a  href="#anchor6.3"></a>
### 6.3 Example of cost-effectiveness expressions

****▼Cost-effectiveness is expressed in terms of time series and period totals.****

The estimated costs and effects can be expressed as a time series or a period total (Figure 6-6). In case of a time series, the costs and effects must be organized by the time of occurrence or manifestation. When expressed as a period total, it is possible to consider costs and effects that cannot be fully covered by annual units like effects of a disaster.

**The effects of a major disaster are not expressed as a time series, but rather as additional effects that may occur during the total period of the disaster, since the occurrence and the time of occurrence are uncertain.

 <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E5%9B%B3%206-6%20%E8%B2%BB%E7%94%A8%E5%AF%BE%E5%8A%B9%E6%9E%9C%E3%81%AE%E8%A1%A8%E7%8F%BE%E4%BE%8B.png?raw=true" width="60%">
 
**Figure 6-6 Example of cost – effectiveness expressions**

In the future, we will examine the cost-effectiveness of a digital twin that includes not only government services but also private services.

<a  id="anchor7"></a>
<a  href="#anchor7"></a>
### 7. Conclusion

The first edition of the roadmap outlines the concept (Chapter 1), vision (Chapter 2), components (Chapter 3), steps (Chapter 4), development and operation (Chapter 5), and cost-effectiveness (Chapter 6) of the urban digital twin that the Tokyo Metropolitan Government aims to realize for social implementation. The study group will discuss these issues in the future.

As a prospect of our project, with receiving opinions from experts in various fields at the study group and reflecting the results of the demonstration project and the results of discussions with various bureaus, specific steps and actions for the development and utilization of a digital twin in a city will be discussed. The roadmap will be also updated successively toward the second edition.

<a  id="anchorReference Glossary"></a>
<a  href="anchorReference Glossary"></a>
###  Reference Glossary

  <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8_%E5%8F%82%E8%80%83%E7%94%A8%E8%AA%9E%E9%9B%86.png?raw=true" width="60%">

<a  id="anchorReferences"></a>
<a  href="anchorReferences"></a>
###  References

The following is an overview of the literature consulted in preparing this roadmap.

  <img src="https://github.com/tokyo-digitaltwin/roadmap_v1.0/blob/images/%E8%A1%A8_%E5%8F%82%E8%80%83%E6%96%87%E7%8C%AE.png?raw=true" width="60%">

1. Smart City Reference Architecture White Paper

In order to accelerate the realization of smart cities and the smooth coordination and distribution of personal data, and to promote the realization of Society 5.0, the Cabinet Office released the first version of the "Strategic Innovation Program (SIP) Phase 2: Cyber Space Infrastructure Technology Architecture Construction and Demonstration Research Project Using Big Data and AI The first version of this paper was published on March 31, 2020 as an outcome of the "Strategic Innovation Program (SIP) Phase 2: Architecture Development and Demonstration Research Project for Cyberspace Infrastructure Technology Using Big Data and AI.

This paper is intended for a wide range of readers, including local governments and companies that are planning to take an active role in smart cities, all companies that are considering providing smart city-related services, and the national government, companies, and academia that are considering the future of smart cities in Japan. By presenting a wide range of components necessary for the promotion of smart cities, including not only systems but also strategies and organizations, this report is intended to serve as a reference for regions and municipalities that are planning to start or expand smart city initiatives to consider what and how to decide on what to do and how to do it. The purpose of this document is to define an urban operating system (OS) as the basic platform for smart cities, and to define the minimum necessary data and authentication exchange rules (API) in the urban OS, so that services and data can be interconnected and efficiently distributed among smart cities. The purpose of the OS is to enable services and data to be interconnected and efficiently distributed among smart cities.

2. Digital Twin Toolkit

The 'Digital Twin Toolkit' is a document published by the Centre for Digital Built Britain (CDBB) in 2021 to assist those considering the need for and uses of a digital twin. As the subtitle states 'Developing the business case for your digital twin', the document also explains use cases and case study methods. Specifically, the 'Digital Twin Toolkit' is composed of a table of contents that describes what a digital twin is, a framework of use cases, case studies, and items to be implemented in order to promote digital twinning. The CDBB is an industry-government-academia partnership funded by the British government and established within the University of Cambridge.

