## hi, i'm asher ♡

<img 
  src="https://wsrv.nl/?url=raw.githubusercontent.com/asleepwithabook/asleepwithabook/main/avatar.png&w=300&h=300&mask=circle"
  align=right>

<div style="padding: 0px;">
  <a href="linkedin.com/asherbruce/"><img alt="LinkedIn Badge" src="https://img.shields.io/badge/LinkedIn-%2Fin%2Fasherbruce%2F-blue?style=flat-square&labelColor=white&color=blue"></a>
  <a><img alt="GitHub followers" src="https://img.shields.io/github/followers/asleepwithabook?style=social&label=follow"></a>
</div>

*Data Science and Political Economy Student at [The College of Idaho](collegeofidaho.edu)*

### about me

```r
asher <- data.frame(
  pronouns          = c("she", "her", "hers"),
  code              = c("R", "Python", "HTML", "CSS"),
  tools             = c("tidyverse", "regex", "Shiny", "tidymodels", "Quarto"),
  statistic_methods = c("Factor Analysis", "ANOVA", "Regression", "PCA")
)
```

<img height="230" alt="What I'm Learning Graphic" src="https://github.com/user-attachments/assets/750c6549-2347-4a4d-9e4b-7d440155a8ea">

### what i'm learning

- **Data visualization in ggraph**
  - *Network analysis*
  - *Factor structure*
- **Data cleaning in tidyverse**
  - *Preprocessing with recipes*
  - *Parsing text with regex*
- **Psychometric methods**
  - *Assessing test validity with exploratory factor analysis*
  - *Scoring tests with item response theory*

## fun things i've made

### [factor analysis on chapman university's american fears survey](https://github.com/asleepwithabook/individual_project)

#### tools

R:
  tidyverse
  psych


#### overview
The Chapman University Survey on American Fears (CSAF) collects data on Americans' fears, attitudes, and behaviors. Using factor analysis, we can see how these categories and the items within them are related.

> *Are all the questions about fear of pollution measuring a "fear of pollution" trait?*  
> *Does news consumption load onto the same factor as perceptions of political selfishness?*

#### process
Survey data tend to be messy. The CSAF doesn't define its own variables, so it didn't mark questions as reverse-scaled. 

After reversing the necessary questions, they need to be labeled so that factors can be correctly identified.

> Q17A doesn't give me enough information to say that a factor is measuring religiosity!

This required parsing the codebook using regex, pulling the question text and possible answers into a readable format.

Once the data is readable, the factor analysis can be performed. I used psych::fa() to perform a hierarchical factor analysis

#### results

#### takeaways
