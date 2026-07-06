# Shapping Viewer's Reality: The Tempo of PTA's Films

## Intro

My aim for this project is to visualize the tempo of each of PTA's films by comparing and compiling data on shot, scene, and movie lengths. Creating a comprehensive breakdown of tempo in each of PTA's films will allow the PT-annotated project to bolster its annotations. Below are two essays written on film tempo and the important role it plays in audience perception of time in film:

[View Impact of Shot Length and Motion on Cinematic Tempo](https://kth.diva-portal.org/smash/get/diva2:1704346/FULLTEXT01.pdf) essentially explains the role of tempo in film and also conducts its own study of action films. The conclusion the essay reaches is that when shot lengths are shorter, the viewer will perceive the film as having a higher tempo. 

[View Study of Shot Length and Motion as Contributing Factors to Movie Tempo](https://dl.acm.org/doi/pdf/10.1145/354384.354530) conducts a study to demonstrate how tempo is used by filmmakers. The study tests the ability of machine learning to see if the machine learning is able to gain important information about the film. The study was successful, and thus the authors conclude that shot length and motion can be used not only to change a film's tempo but also to convey meaningful information to viewers. 

Having a part of the PTA-annotated website dedicated to tempo would not only help to improve viewers' understanding of the inner workings of film but also may provide them further insight into the messages of the films. In our film analysis workshop, we learned how important the way things are shot allow the audience to gain information/make assumptions about a film (even when only given two minutes out of a two-hour film). A fast tempo can make the audience feel nervous, discombobulated, etc. While a slow tempo can make things feel more dramatic or mundane given the context. This then can make the viewer think: how does PTA use tempo to make his audiences feel? Is he successful with his use of tempo? Why do some of PTA's films have quicker/slower tempos?

## The Data

I have already begun to compile data from the PTA annotations by calculating the length of each scene in PTA's films. I used the scene-list time stamps chosen by the PTA team and converted each scene length to seconds. It's worth mentioning that the calculated scene lengths are not accurate to the films themselves due to a multitude of factors: scenes with many screenshots (lots of camera changes, motion, etc) typically were made shorter to make the screenshoter's job easier; the scenes were given more equal divisions to make work easier to divide amongst screenshoters; etc. 

From this data, I calculated the average length of all scenes in PTA's films, the average length of each scene of every individual film, and the longest/shortest scene/movie.

### Data Visualizations Thus Far

Below are some of the graphs I've made so far:

![Breakdown of PUNC scenes length + total #](Presentation/Slide1.jpg) 
![Breakdwon of PHAN scenes length + total #](Presentation/Slide2.jpg)
![Breakdwon of LICO scenes length + total #](Presentation/Slide3.jpg)
![Breakdwon of BOOG scenes length + total #](Presentation/Slide4.jpg)
![Breakdwon of INHE scenes length + total #](Presentation/Slide5.jpg)
![Breakdwon of MAGN scenes length + total #](Presentation/Slide6.jpg)
![Breakdwon of MAST scenes length + total #](Presentation/Slide7.jpg)
![Breakdwon of HARD scenes length + total #](Presentation/Slide8.jpg)
![Breakdwon of TWBB scenes length + total #](Presentation/Slide9.jpg)
![Breakdwon of OBAA scenes length + total #](Presentation/Slide10.jpg)
![Breakdwon of all film scenes length + total #](Presentation/Slide11.jpg)
![Breakdwon of the average scene length across all films](Presentation/Slide12.jpg)

I think these graphs are interesting because they are representative of the different opinions of what constitutes a scene in the opinion of the people dividing them up. I also think that given more data, we could start to develop some interesting analysis of trends in film length affecting number of scenes and length of scenes, etc. 

## Future Data Visualizations

Below are some hand-drawn graphs I hope to create if I continue on with this project:

![More visually engaging way to present breakdown of film scenes length](Presentation/IMG_9352.png)

![More graph ideas plus a strip plot](Presentation/IMG_9353.png)

![Another strip plot graph](Presentation/IMG_9354.png)

## Continuing Research

I would like to work with computer vision and also acquire the length of every shot in PTA's work. This way, I can create visualizations that provide a clearer breakdown of how time operates within PTA's films. I am planning on using Distant Viewer Explorer to accomplish this. I also want to create more scene breakdown graphs comparing the scene times I've been provided and the "official" scene times using scripts and watching the films. 

