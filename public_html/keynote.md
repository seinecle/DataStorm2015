The nice thing about fields in computational science is that they evolve so quickly. Every 6 months or so, there is a new kid on the block in machine learning, mobile app development or text mining.  
This makes it hard to stay at the forefront of these fields, and sometimes we might even loose perspective as to the meaning and goals of what was the field we formed an interest in, a couple of years back.  

In this talk, I'd like to explore how data visualization has evolved, and keeps evolving as a field. Some warnings. I am more an observer than a participat in this field. My view is the one of somebody who came to data visualization around 2009 through network visualizations with Gephi, getting my information mostly from the discussions of data visualizers which I follow and interact with on Twitter. These are personal views and I'd be happy to see them (productively) challenged.  

So I feel that in the last 6 years, there is an evolution in dataviz: it came to age, lived happily through a golden age, and we are today somewhere else. Let's start with the beginning.  

Before dataviz, there was a couple of established fields of practice dealing with graphics and data. I'll mention 4 of them though there are others:
infoviz, Business intellegience, infographics, and GIS.  

1. Infoviz is "information visualisation" and is the name of an academic field concerned with "the study of (interactive) visual representations of abstract data to reinforce human cognition." (Wikipedia entry). The strength of this field is that it is a test bench for many assumptions you'd have on how visualizations can be effective, in terms of "reinforcing human cognition". How do colors work? What about different scales? Are users performing at some given tasks when reading graph structures representated as matrix, versus networks? Should longitudinal data be presented as time slices or animated movies for best understanding? Research in information visualization is concerned with providing solid answers to these important questions. The issue is, this emphasis on hypothesis testing can be detrimental to the advancing on the bigger picture: creating visualizations that are engaging and trigger adoption by the viewer. To be a bit tough on infovis, I'd say you need a PhD to get it: the interfaces they design are not user friendly, and the information displayed hardly enhances human cognition for laymen like me.  

2. You could say that infographics is a bit the contrary of infovis: communication agencies doing pretty much what they want to catch the attention of their readers, at the expense of truthfulness and reliability of the data they invoke. Of course there are excellent infographics and Alberto Cairo, a professor and journalist by trade, reminds us in his book "The Functional Art" that carefully executed infographics are an excellent way to convey complex information in a limited amount of space. But my understanding is that it is not in the basic contract of infographics to have a one to one relation with data, there is a license to *illustrate* the data. The reader must trust the source of the infographics much more than in information visualisation: depending on whether this is a communication agency or an established newspaper (and even then!), infographics can be misleading.  

3. Business intelligence is still another crowd: the mission is basically to go "beyond excel" in terms of reporting and monitoring business data. Nothing fancy usually there: bar charts, pie charts, line charts and progress bars assembled in dashboards, sold by companies more versed in the business side of things than graphics.  

4. And finally, GIS.  

So the scene is this one: scientists in their corner being the guardians of the temple of "proper visualisations", but they have a hard time finding an audience for these graphics. Infographics in the opposite corner, who have access to crowds of readers everyday in the pages of newspapers and marketing brochures, but with a sense that they don't really show the data - they editorialze it a lot, for good or bad. And at the two other corners, we have business intelligence which is a bit scorned upon because of the simplicity of their graphics which does not do justice to the richness of the data, but envied because they have access to relevant, pricey, impactful data. And GIS which works with data in a way which is universally understood and judged relevant (maps), though the degree of innovation remained quite low.  

And then something happened around 2008 and 2009, so around 6 years ago:  
- a number of javascript charting and drawing libraries were released: RaphaelJS (08/08/08), the Javascript Infovis Toolkit (2009), Protovis (2009), ProcessingJS (2010), D3 (2011). Together with the take off of mobiles phones without the Flash and Java plugins, the decreasing popularity of the Java plugin even on desktop browsers, you see in 3 years a large technological shift: unification of visualization frameworks on the web using javascript. The web becomes increasingly a platform in itself (more popular than releasing desktop software), with the release of Google Chrome in 2008 - Javascript and CSS become much less broken than when Internet Explorer was dominant. For what impact?  

It shuffled the cards: with Java came a very rigid way to conceive interfaces: windows, menus and even the fonts had a Java look and feel in the browser. In Flash, you had a strong history of interaction and feel for design, but you could use Flash without coding, so that Flash designs could remain pretty much disconnected from the datasets they represented. All that became thrown into the melting pot of Javascript where everybody had to unlearn their framework and learn on a virgin land.  

And what happened was a solidification of a community around a couple of features:

1. Data is for the viewer to see and play with  
There is the assumption that the visualization should not provide you with flat and unverifiable conclusions: it should show the data in a transparent form. Of course there is a narrative and an editorialization of how the datais presented, **but** it always remains possible for the viewer to challenge this editorial view because the data is here for anyone to explore and interact with.
This represents a fundamental break with infographics, which can hide the underlying data by design, or show it with strong bias by carelessness and still be "OK" by pre-dataviz standards. It is also a break with infovis, were data is indeed there but you need a book length user guide to actually get to it.

2. Custom made, creative act  
Because we are in the browser there is no click and point solutions for the visualization of the data. This departs strongly from GIS where "custom" maps could be done by selecting options in a menu, and also a big change from dashboards in business intelligence where you could drag and drop charts to build a visualization. The sense of esthetics and the particularity of the datasets makes of each dataviz a craftwork.  


What was remarkable was that "dataviz" happened at the interface of different communities, it was not the natural offspring of one of the 4 I mentioned. What you got was:
    
1. Individuals possessing a mix of coding skills for the preparation of the data (Python or R skills), skills in javascript and other scripting language for visual design (ActionScript, Processing), a knowledge of the rules of design and a feel for esthetics, and creativity.

2. A tight knit group : Santiago Ortiz, Jerome Cukier, Jer Thorp, Gregor Aisch, Jan Willem Tulp, Lynn Cherny, Nathan Yau from Flowing Data, Kim Rees, Moritz Stefaner, with a couple of established academics like Enrico Bertini and Jon Schwabish, and in relation with teams at the Guardian and the NYT, and Andy Kirk VisualisingData as an evangelist and instructor.

3. Twitter based communication around the "dataviz" hashtag, where people exchanges praises and criticisms, shared their latest realization and the chat about past and upcoming conferences.

From there on, #dataviz was a launched with:
- a couple of emblematic projects: OECD Better Life Index: not infovis, not infographics, just dataviz:  
<p align="center"><img src="img/formatted/oecd better life index.jpg"/></p>  

- the "Ghost Counties" visualization by Jan Willem Tulp, 2011: http://www.janwillemtulp.com/eyeo/:  
<p align="center"><img src="img/formatted/ghost counties screenshot.jpg"/></p>  

- U.S. Gun Deaths by Periscopic, http://guns.periscopic.com/?year=2013  
<p align="center"><img src="img/formatted/gun deaths.jpg"/></p>  


The emergence of data visualisation as a set of practice and professionals was coinciding with the surge in the new importance of data as a driver of value for business. "Data visualization" became positioned as one powerful lever to extract value from datasets: it possesses both the rigor needed to report objectively on key data features, that you'd find otherwise in information visualisation, and the power to be engaging with the domain specialists or the managers in charge of finding insights in the data.

Two aspects where data visualization epitomizes its value: maps and networks.  
Visualization of geolocalized data and of network data has of course a long history before the birth of data visualization: many software integrated mapping functions from Geographical Information Systems, and network analysis packages also add visualization add-ons.  

What data visualization brought was staggering visualizations making engagement with data just stronger, more powerful. Stamen, an agency with strong ties in the data visualization community, does this kind of maps:  
<p align="center"><img src="img/formatted/stamen.jpg"/></p>  

http://prettymaps.stamen.com/201008/#10.00/38.7250/-9.1500  
Not your usual GIS mapping.  

In terms of networks, a pre-dataviz typical network would look like:  
<p align="center"><img src="img/formatted/ucinet.jpg"/></p>  


Dataviz brought interaction, web-based interactions - which means you explore the viz, not just stare at it, javascript as a common language, and a strong sense of esthetics.
http://bl.ocks.org/mbostock/1062288  


<p align="center"><img src="img/formatted/logos bi.png"/></p>  
Industrialization came in rapidly, with Tableau becoming the leader for general purpose viz, dashboards reinvented themselves in dataviz-style with Bime, Qlik, Palantir to name a few.  

Dataviz became integrated into the business discourse on big data: the Harvard Business Reviews features in 2012 a blog section on data visualization where Jer Thorp contributed to set perspectives straight on data,  
<p align="center"><img src="img/formatted/jer thorp.jpg"/></p>  



, Nielsen branded their annual report with a dataviz created by Jan Willem Tulp, GE did ????

So until 2013, 2014 I'd say that we were in the golden age of #dataviz: excited comments on new productions by the NYT, debates around the goals of #dataviz: is it a way to tell stories? To open new worlds? New connections made with new comers, new agencies, people meeting for the first time in conferences after exchanging on Twitter for years, new positions, big clients...

And in 2015, things seem to have stopped a bit. Dataviz is still there of course, but the energy has changed. The conversation on Twitter has slowed down a lot. The sense of being pionneers has eroded, because time has passed and because we have indeed tried and explored many low hanging fruits. Many individuals are now engaged in more industrial, long term projects. So that's not bad news: dataviz is now mainstream and well established, people are less obliged to enter free competitions and release long personal projects to get their name out, that's good. But I miss a bit the excitement of the previous years when you had one framework and one big personal project published per month.

So... where is dataviz going? I have some ideas on that. As I said, you have this first exciting phase that passed, and we are now in a stage where processes for the creation of dataviz are more industrialized, commodified, stabilized. This means that innovation will find other places to erupt. Why? Because the landscape of technologies keep changing, and creative minds will seize the opportunity to play and explore these opportunities.







End of dataviz: obstacles
Big data viz? Ok, but far from democratic technos, slows down development
Big bucks? Yes, but that is embedded in big bucks companies, less fun (Tableau...) less far west-y

Next frontier: outside of screens. Find the maker spirit elsewhere: objects, wearables, sculptures...








