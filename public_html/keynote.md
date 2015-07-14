#Where is data visualization going?
by [Clement Levallois](http://www.clementlevallois.net), DataStorm 2<sup>nd</sup> edition, Lisbon, July 15, 2015.  

The nice thing about fields in computational science is that they evolve so quickly. Every 6 months or so, there is a new kid on the block in machine learning, mobile app development or text mining.  
This makes it hard to stay at the forefront of these fields, and sometimes we might even loose perspective as to the meaning and goals of what was the field we formed an interest in, just a couple of years back.  

So I took the opportunity of this talk to reflect on data visualization, which is such a young field. I'd like to explore how data visualization has evolved, why there was a need for it to emerge, where it stands today, and I will try to imagine where it will evolve in the coming years.  
Some warnings. I am more an observer than a participat in this field. My view is the one of somebody who came to data visualization around 2009 through network visualizations with Gephi, getting my information mostly from the discussions, links and podcasts shared by data visualizers which I follow and interact with on Twitter. These are personal views and I'd be happy to see them (productively) challenged.  

So I feel that in the last 6 years, there is an evolution in dataviz: it came to age, lived happily through a golden age, and we are today somewhere else. Let's start with the beginning.  


##Before dataviz
Before dataviz, there was a couple of established fields of practice dealing with graphics and data. I'll mention 4 of them though there are surely important others:
infoviz, infographics, Business intelligence, and GIS.  

###1. Infoviz
Infoviz is "information visualisation" and is the name of an academic field concerned with "the study of (interactive) visual representations of abstract data to reinforce human cognition." (Wikipedia entry). The strength of this field is that it is a test bench for many assumptions you'd have on how visualizations can be effective, in terms of "reinforcing human cognition". How do colors work? What about different scales? Are users performing at some given tasks when reading graph structures representated as matrix, versus networks? Should longitudinal data be presented as time slices or animated movies for best understanding? Research in information visualization is concerned with providing solid answers to these important questions.  
<p align="center"><img src="img/formatted/example infovis.jpg"/></p>  

The issue is, this emphasis on hypothesis testing can be detrimental to the advancing on the bigger picture: creating visualizations that are engaging and trigger adoption by the viewer. To be a bit tough on infovis, I'd say you need a PhD to get it: the interfaces they design are not engaging, not user friendly, and the information displayed hardly enhances human cognition for laymen like me.  

<p align="center"><img src="img/formatted/example infographics.jpg"/></p>  
###2. Infographics  
You could say that infographics is a bit the contrary of infovis: communication agencies doing pretty much what they want to catch the attention of their readers, at the expense of truthfulness and reliability of the data they invoke. Of course there are excellent infographics and Alberto Cairo, a professor and journalist by trade, reminds us in his book "The Functional Art" that carefully executed infographics are an excellent way to convey complex information in a limited amount of space. But my understanding is that it is not in the basic contract of infographics to have a one to one relation with data, there is a license to *illustrate* the data. The reader must trust the source of the infographics much more than in information visualisation: depending on whether this is a communication agency or an established newspaper (and even then!), infographics can be misleading.  

###3. Business intelligence is still another crowd:  
<p align="center"><img src="img/formatted/example bi.jpg"/></p>  
The mission is basically to do "excel-level" visualizations in terms of reporting and monitoring business data. Nothing fancy usually there: bar charts, pie charts (often in 3D, which is wrong), line charts and progress bars assembled in dashboards, sold by companies more versed in the business side of things than graphics and innovation in design.  

###4. And finally, GIS.  
<p align="center"><img src="img/formatted/gis.jpg"/></p>  
Geographical Information Systems can have a claim for the longest tradition of visual data, this is after all their business to draw maps which is geolocalized data. It could be that this long tradition was also a curse: because they developped these widely used desktop software in the 1990s and the 2000s, they were entrenched in technologies that could not be easily adapted when web technologies became the de facto standard to draw maps and to project overlays of data on them.  

So the scene is the following: scientists in their corner being the guardians of the temple of "proper visualisations", but they have a hard time finding an audience for these graphics. Infographics in the opposite corner, who have access to crowds of readers everyday in the pages of newspapers and marketing brochures, but with a sense that they don't really show the data - they editorialze it a lot, for good or bad. And at the two other corners, we have business intelligence which is a bit scorned upon because of the simplicity of their graphics which does not do justice to the richness of the data, but envied because they have access to relevant, pricey, impactful data. And GIS which works with data in a way which is universally understood and judged relevant (maps), though the degree of innovation of this field remained quite low.  

## The emergence of dataviz
Something happened around 2008 and 2009, so around 6 years ago, which changed this statu quo:  
- a number of javascript charting and drawing libraries were released: RaphaelJS (08/08/08), the Javascript Infovis Toolkit (2009), Protovis (2009), ProcessingJS (2010), D3 (2011). Together with the take off of mobiles phones without the Flash and Java plugins, the decreasing popularity of the Java plugin even on desktop browsers, you see in 3 years a large technological shift: unification of visualization frameworks on the web using javascript. The web becomes increasingly a platform in itself (more popular than releasing desktop software), with the release of Google Chrome in 2008 - Javascript and CSS become much less broken than when Internet Explorer was dominant. For what impact?  

It shuffled the cards: with Java came a very rigid way to conceive interfaces: windows, menus and even the fonts had a Java look and feel in the browser. In Flash, you had a strong history of interaction and feel for design, but you could use Flash without coding, so that Flash designs could remain pretty much disconnected from the datasets they represented. All that became thrown into the melting pot of Javascript where everybody had to unlearn their framework and learn on a virgin land.  

And what happened was a solidification of a community around what I see as 2 defining traits:

###1. Data is for the viewer to see and play with  
There is the assumption that the visualization should not provide you with flat and unverifiable conclusions: it should show the data in a transparent form. Of course there is a narrative and an editorialization of how the datais presented, **but** it always remains possible for the viewer to challenge this editorial view because the data is here for anyone to explore and interact with.
This represents a fundamental break with infographics, which can hide the underlying data by design, or show it with strong bias by carelessness and still be "OK" by pre-dataviz standards. It is also a break with infovis, were data is indeed there but you need a book length user guide to actually get to it.

###2. Custom made, creative act  
Because we are in the browser there is no click and point solutions for the visualization of the data. This departs strongly from GIS where "custom" maps could be done by selecting options in a menu, and also a big change from dashboards in business intelligence where you could drag and drop charts to build a visualization. The sense of esthetics and the particularity of the datasets makes of each dataviz a craftwork.  
One of the best examples is this one by Hint.fm: 
<p align="center"><img src="img/formatted/windmap.jpg"/></p>  
(live url: http://hint.fm/wind/)  
(live url for a worldwide version: http://earth.nullschool.net/)  


What was remarkable was that "dataviz" happened at the interface of different communities, it was not the natural offspring of one of the 4 I mentioned. This community is remarkable in several aspects:
    
###1. Individuals possessing a mix of skills:
For the preparation of the data (Python or R skills), skills in javascript and other scripting language for visual design (ActionScript, Processing), a knowledge of the rules of design and a feel for esthetics, and creativity.
That is what you need to create this:  
<p align="center"><img src="img/formatted/mta.jpg"/></p>  
(live url: http://www.mta.me)    


###2. Twitter based communication around the "dataviz" hashtag
In this community, people evaluate each other's works, shared their latest realization chat about past and upcoming conferences but more importantly exhchange info about new frameworks and resources.  

<p align="center"><img src="img/formatted/clark.jpg"/></p>  
(live url: http://neoformix.com/2012/DataVisFieldSubGroups.html)    

###3. A tight knit group across the US and Europe.
I identify Santiago Ortiz, Jerome Cukier, Jer Thorp, Gregor Aisch, Jan Willem Tulp, Lynn Cherny, Nathan Yau from Flowing Data, Kim Rees from Pseriscopic, Moritz Stefaner, with a couple of established academics like Enrico Bertini and Jon Schwabish, and in relation with teams at the Guardian and the NYT, and Andy Kirk at VisualisingData as an evangelist and instructor.  
<p align="center"><img src="img/formatted/dataviz group.jpg"/></p>  
(live url: http://neoformix.com/2012/DataVisField1000_Group2.pdf)    


From there on, #dataviz can be described by a couple of emblematic projects:
- OECD Better Life Index by Moritz Stefaner et al: not infovis, not infographics, just dataviz: simplicity, interaction, access to the data.   
<p align="center"><img src="img/formatted/oecd better life index.jpg"/></p>  
(live url: http://www.oecdbetterlifeindex.org/)    

- the "Ghost Counties" visualization by Jan Willem Tulp, 2011: shows creativity and engagement.  
<p align="center"><img src="img/formatted/ghost counties screenshot.jpg"/></p>  
(live url, needs Internet Explorer and Flash: http://www.janwillemtulp.com/eyeo/)    

- U.S. Gun Deaths by Periscopic, http://guns.periscopic.com/?year=2013  
<p align="center"><img src="img/formatted/gun deaths.jpg"/></p>  
(live url, needs Internet Explorer and Flash: http://guns.periscopic.com/?year=2013)  

The emergence of data visualisation as a set of practice and professionals was coinciding with the surge in the new importance of data as a driver of value for business. "Data visualization" became positioned as one powerful lever to extract value from datasets: it possesses both the rigor needed to report objectively on key data features, that you'd find otherwise in information visualisation, and the power to be engaging with the domain specialists or the managers in charge of finding insights in the data.

###Two aspects where data visualization epitomizes its value: maps and networks.  
Visualization of geolocalized data and of network data has of course a long history before the birth of data visualization: many software integrated mapping functions from Geographical Information Systems, and network analysis packages also add visualization add-ons.  

What data visualization brought was staggering visualizations making engagement with data just stronger, more powerful. Stamen, an agency with strong ties in the data visualization community, does this kind of maps:  
<p align="center"><img src="img/formatted/stamen.jpg"/></p>  
(live url: http://prettymaps.stamen.com/201008/#10.00/38.7250/-9.1500)  
Not your usual GIS mapping! What this kind of map brings is: interaction, accessibility, and most of all enhanced **engagement** with the viewers.

In terms of networks, a pre-dataviz typical network would look like:  
<p align="center"><img src="img/formatted/ucinet.jpg"/></p>  

Dataviz brought interaction, web-based interactions:
<p align="center"><img src="img/formatted/d3 force layout.jpg"/></p>  
(live url: http://bl.ocks.org/mbostock/1062288)  

This type of visualization means you can explore the viz, not just stare at it, you can share it - just paste the url. It can be developed and modified by a large pool of developers because it is written in javascript, which is  the common language of web development. There is a strong sense of esthetics and natural feeling using it. It will encourage curiosity, exploration, and just increase 10 folds the time spent on it.  

A short note on Gephi here: Gephi is a desktop software developed in Java. This contributes to explain why it takes years to release the next version of Gephi, as compared to development cycles that are measured in months for javascript dataviz frameworks. I hope Gephi will overcome this weakness.  

##2014-2015: The stabilization of #dataviz
Anyhow, industrialization in dataviz came in rapidly, with Tableau becoming the leader for general purpose viz, dashboards reinvented themselves in dataviz-style with Bime, Qlik, Palantir to name a few.  
<p align="center"><img src="img/formatted/logos bi.jpg"/></p>  

Dataviz became integrated into the business discourse on big data: the Harvard Business Reviews features in 2012 a blog section on data visualization where Jer Thorp contributed to set perspectives straight on data,  
<p align="center"><img src="img/formatted/jer thorp.jpg"/></p>  
(live url: https://hbr.org/2012/11/data-humans-and-the-new-oil/)  


Nielsen, the leader of market data and market research, worked on its corporate identity to include data visualization, with data-driven visuals custom made by Jan Willem Tulp:
<p align="center"><img src="img/formatted/nielsen.jpg"/></p>  

Since 2012 or so, General Electric partners with Fathom, the agency created by Ben Fry (creator of Processing!) to create visualizations relative to their corporate identity, with some impressive realizations:
<p align="center"><img src="img/formatted/ge.jpg"/></p>  
(live url: http://visualization.geblogs.com/visualization/powering/)  

And in 2015, you know dataviz has gotten to a pinacle when you see a panel on dataviz with Ben Fry and Chelsea Clinton:
<p align="center"><img src="img/formatted/chelsea.jpg"/></p>  
(live url: https://www.youtube.com/watch?v=YFrmQDCpgxs)  


So until 2012 and 2013 I'd say that we were in the golden age of #dataviz in terms of discovereries and charting new paths: excited comments on new productions by the NYT, debates around the goals of #dataviz: is it a way to tell stories? To open new worlds? To educate? New connections made with new comers, new agencies, people meeting for the first time in conferences after exchanging on Twitter for years, new positions, big clients...

And in 2015, things seem to have stabilized and normalized. The energy has changed. The conversation on Twitter has slowed down a lot. The sense of being pionneers has eroded, because time has passed and because we have indeed tried and explored many low hanging fruits. Many individuals are now engaged in more industrial, long term projects. So that's not bad news: dataviz is now mainstream and well established, people are less obliged to enter free competitions and work on long personal projects at weekends and nights to get their name out, that's good. But I miss a bit the excitement of the previous years when you had one framework or one big personal project published per month, and when you had all these big shots chatting on Twitter about the upcoming developments for dataviz.

## 2015 onwards: where is dataviz going?
So... where is dataviz going? As I said, you have this first exciting phase that passed, and we are now in a stage where processes for the creation of dataviz are more industrialized, commodified, stabilized. This means that innovation will find other places to erupt. Why? Because the landscape of technologies keeps changing, and creative minds will seize the opportunity to play and explore these opportunities in places where no "client" is yet waiting for them.  

To illustrate possible paths, I like to give the example of the career of Seb Lee Deslile, who defined himself as a creative coder and now as as a digital artist. I follow his work on Twitter since about 2009. He is not at the heart of the "dataviz" network and does not define himself in regards to this label, but you'd find him on Jeff Clark's map of dataviz in 2012 nonetheless.  

- so, he was using Adobe Flash as one of his main technologies until 2009, contributing to PaperVision3D, a framework to build 3D games and animations in the Flash Player.  
- He plays a bit with Adobe Flex in 2009,  
- in 2010, he moves to HTML5 technologies, using and teachig animated graphics in Javascript  
- in 2012, he does the lunar trail project: http://seb.ly/work/lunar-trails/
- in 2013, he does pixelpyros: http://pixelpyros.org/  
- in in 2014/2015, he launches workshops on "Stuff that talk to the Internets": http://seb.ly/st4i-stuff-that-talks-to-the-interwebs/  

This path, and similar paths followed by others, suggest that:

1. The computer screen and even the screen of the mobile phone is becoming less hegemonic as the medium where data can be visualized. Objects, sculptures, buildings, furniture... this is the next frontier to be explored. Not just mapping data on a flat surface, but maybe even actual construction of data objects.     

2. Interaction is richer than we are used to. When we leave the "screen" environment (desktop of mobile), interactions with the user become more diverse. Not just the hand, but the body. Not one individual facing an object, but possibly a crowd, possibly moving, possibly gesturing. 

3. And "data" is in the process of getting an even larger meaning. I mean, I was happy to move from a tabular notion of data to "unstructured text": like wow, that opens wild possibilities! But when you move away from the screen and start connecting to a variety of ojbects, sensors, and with a variety of people, data takes still other forms: real time measurements from the external physical environment, from the internal (body) environment, from local or distant social interactions as they unfold, ... 

If visualizing data from the Twitter API was the cliché of #dataviz in 2010 - 2015, the next cliché could be the instantaneous 3D printing of data generated from the connected objects and bodies in a home or a workspace .  

This is just a vision for dataviz, I'd be happy to discuss it with you now!  









