
# Projects & Achievements


## Table of Content :books: 
- Let's talk Data Science
    - Flight delay forecast
    - What's the next hit song?

- Teachings
    - Why is Machine Learning fun
    - Make people love Data

- My journey at MBCME
    - Automation & Optimisation
    - Data Analytics


---

## Who am I?👩‍🔬👩‍🏫🧗‍♀️

- Graduated from Business and Engineering Schools
- Data Scientist
- Sports Lover

---

## Let's talk Data Science.

### Helicopters Data Scientist :helicopter: 

<div align = "center">

<img align="center" src = "https://airbus-h.assetsadobe2.com/is/image/content/dam/products-and-solutions/formation-flight/Airbus-Helicopter-family-flight-Marignane-006.jpg?wid=1920&fit=fit,1&qlt=85,0" width='500'>

<br>


<img align="center" src = "https://img.evbuc.com/https%3A%2F%2Fcdn.evbuc.com%2Fimages%2F34444498%2F113026609461%2F1%2Foriginal.jpg?auto=compress&s=39dfa86c5253bda45a0b348fd68d38f2">

</div>

---

### Flight delay predictions :airplane: 

<br>

:::info
Business case: How to forecast flight's delay? ⏰
:::

<img align="center" src= "https://i.stack.imgur.com/2fBD5.jpg" width ='500'>

<br>
<br>

**A regression problem:**

- 🎯 **Objective**: Predict the arrival delay

- 📋 **Dataset**: 5 million rows - 65 features
- 🔎 **Cleaning & processing**: Temporal, Geographical, categorical, numerical data
- 🤖 **Modeling**: Linear Regression, Ridge/Lasso, Boosting methods
- 📈 **Results:** :deciduous_tree:   9 min prediction error


<br>

```typescript
// Create a user-friendly app with Flask
from modele import predict_vol, aero
from flask import Flask, render_template, request
app = Flask(__name__)
```

:::info
Check project:
https://github.com/MarineJL/Flight-Delay

Check app:
https://projet4-marine.herokuapp.com
:::

***

### What's the next hit song? :notes: 


<br>

:::info
Business case: How to predict the hit potential of a song? :musical_score: 
:::

<img align="center" src= "https://static-cashmusic.netdna-ssl.com/www/img/article/lp2.png" width='500'>
<br>
<br>

**A classification problem:**

- 🎯 **Objective**: Predict the hit potential of a song
- 📋 **Dataset**: Built with Spotify API
- 🤖 **Modeling**: Logistic, Penalized regression, Boosting methods
  
- 📈 **Results:** Type I error & Power of Marketing :moneybag:

<br>

<center>

|   |   Not a hit |    Hit      |  Class error |
|----------|:----------:|:-------------:|------:|
| **Not a hit** |  29 | 60 |0.674
| **Hit** |    21   |   129 |0.078

**Confusion Matrix**

</center>

<br>

:::info
Check tutorial:
https://github.com/MarineJL/Spotify_Data

Check thesis:
https://github.com/MarineJL/MasterThesis
:::
---
## Teachings 👩‍🏫
 
### Why Machine Learning is fun 

<br>

:::danger
🚨 Sensitive topic coming
:::
:::info
Check Viz :soccer: : https://public.tableau.com/profile/marine.jl#!/vizhome/Datavizfifa2/Tableaudebord1
:::

<br>

### How to make people love data


How to predict John Snow's death?
<br>

<p align='center'><img src="https://media.giphy.com/media/J5mja8de1j4Fa/giphy.gif" width='400'></p>
<p align='center'><img src="https://s3.amazonaws.com/dev.assets.neo4j.com/wp-content/uploads/20170716015001/graph-of-thrones.png"></p>


---

## My journey at Mercedes-Benz Cars Middle East.

### Automation & Optimisation

#### Before Automation

<p align='center'><img src="https://media.giphy.com/media/lJnAXeJO8tE7E37mxq/giphy.gif"></p>

<br>

#### A new process

```graphviz
digraph {
  compound=true
  rankdir=LR

  graph [ fontname="Source Sans Pro", fontsize=20 ];
  node [ fontname="Source Sans Pro", fontsize=18];
  edge [ fontname="Source Sans Pro", fontsize=12 ];


  subgraph core {
    c [label="Daily Data \nFlow"] [shape=plaintext]
    d [label =  "Data Base"] [shape = box]
    e [label = "Raw Data"] [shape = box]
    f [label = "Data cleaning and processing"] [shape = "rarrow"]
    c -> d [constraint=false]
    d -> e [label = "extract files \n as .txt"] [constraint=false]
    e -> f  [label = "Python + VBA"] [constraint=false]
    f->a
f ->b 
}

  subgraph cluster1 {
     concentrate=true
    a [label="email"] [shape=box]
    b [label="Dasboard"] [shape=box]
    label="Daily Report"
  }
  
 
 
}
```

#### After Automation
<p align='center'><img src="https://media.giphy.com/media/JIX9t2j0ZTN9S/giphy.gif" width='300px'></p>


***

### Data Analytics

:::warning
:warning:  For confidentiality concerns figures have been modified.
:::

![](https://raw.githubusercontent.com/marinejl/Assigment/master/imgs/PBI1.PNG)
***
![](https://raw.githubusercontent.com/marinejl/Assigment/master/imgs/PBI2.PNG)
***
![](https://raw.githubusercontent.com/marinejl/Assigment/master/imgs/PBI3.PNG)
***
![](https://raw.githubusercontent.com/marinejl/Assigment/master/imgs/PBI5.PNG)

---


<br>


### Thank you! :rocket: 


