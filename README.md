## Project Overview 📊
This project is an analysis made over Music and Mental Health Survey (CC0: Public Domain) dataset, using Python and Tableau. The original dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/catherinerasgaitis/mxmh-survey-results/data)
> "The MxMH dataset aims to identify what, if any, correlations exist between an individual's music taste and their self-reported mental health. Ideally, these findings could contribute to a more informed application of Music Therapy or simply provide interesting sights about the mind."

This data analysis project aims not only to make statements about the findings, but also to raise further questions about the relationship between music and mental disorders, based on the responses to the survey.
### Interpreting Data:
* **Background questions:** Respondents had to answer general questions such as age, whether or not they compose music, primary streaming service they use, hours per day they listen to music, etc.
* **Music Genre:** Respondents were asked to rank how often they listen to 16 music genres, from 'Never' to 'Very Frequently'. They were also asked to identify their favorite music genre.
* **Mental health:** Four mental disorders were considered, and respondents were asked to rate from 0 to 10 how often they experience these disorders/how extreme they find these disorders to be:
  * Anxiety
  * Depression
  * Insomnia
  * OCD

  They also had to answer whether or not music therapy helps them ease their issues.

## Tools 🧰
* Python - Data exploration and cleaning
* Tableau - Data analysis and visualization

## Data Cleaning/Preparation 🧹📂
* Data loading and inspection
* Handling missing values by deletion
![Percentage of null values - Original dataset](https://github.com/ZunigaGarcia/MusicAndMentalHealth-Analysis/assets/168041126/4e443459-3768-4ac7-9cb3-f47bb6bc1eea)
* Handling outliers by Interquartile Range 
* Handling left missing values by imputation
* Final steps and export into a clean format

## Exploratory Data Analysis ❔
EDA involved exploring the data to answer key questions such as:
* How useful is music therapy as a function of the respondents' musical tastes?
* Who are the most vulnerable populations?
* How are mental disorders distributed according to the respondents' taste?

## Dashboards
These can be found in the "Music And Mental Health.twb" file, which I have left along with the other sources in this repository so that you can explore and interact with them. (I do not own Tableau Server so I couldn't upload it there :( ) they are on the very first pages of the Tableau file.
![Dashboard - General Aspects](https://github.com/ZunigaGarcia/MusicAndMentalHealth-Analysis/assets/168041126/217e1d70-1e34-4c96-ab34-43caa172daa8)
![Dashboard - Music effects on Mental Disorders](https://github.com/ZunigaGarcia/MusicAndMentalHealth-Analysis/assets/168041126/ab842b86-6f23-47a1-9a02-5e4450adde56)

## Results/Findings 🔎
1. The most common disorder is Anxiety, followed by depression, being Insomnia an OCD the least common.
2. Particularly with video game music listeners, there were respondents who reported worsening in any of four disorders
3. The Lofi listeners were the ones who showed the highest levels of affectation overall. This leads to the question of whether this musical taste is a cause or causal to these levels of affect.
4. The most affected people are in their early 20's.
5. The older are the least affected people, who just tend to suffer from insomnia.
6. Most people reported to improve from Music Therapy (Aproximately 3/4 of the population)
7. Looking at the effects of music in terms of the participants' favorite genres, it is striking that those who listened to classical music reported getting worse, raising the question of whether this could be due to the often soft and/or melancholic melodies.
8. K-pop listeners are the most likely to suffer from anxiety, which is **worrying** since they are mostly minors.
9. Spotify is the most used streaming service.

## Recomendations 📄
Based on the analysis, we recommend the following actions:
1. Since Spotify is the most popular service, it might be interesting for them to explore a way to recommend some previously made playlists of a particular genre based on how the person reports to be feeling lately, to make that easier.
2. Avoid video game music if you have a recent history of anxiety, depression, insomnia, or obsessive-compulsive disorder.
3. Since most people reported improvement and those most affected were young people, it may be interesting to explore the field of music therapy further and promote it to reach more people.
4. Gospel and Lofi seem to work best for insomnia.
5. Take a closer look at the case of Lofi music, since its listeners are the most affected.

## Limitations 🚦
As shown above, almost 15% of the rows in the dataset were null regarding the 'BPM' column, this being due to it being a more technical field, plus it being slightly skewed, I decided to fill it using the median statistic.
There were some outliers that seemed to be there due to an initial error (e.g.: BPM = 99999.0), but they were handled correctly using the interquartile range technique.

Thanks for reading, remember to check out the code and the Tableau file to take a closer look at this analysis. 🙋‍♂️
