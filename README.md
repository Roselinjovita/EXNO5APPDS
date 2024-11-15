# EXNO5APPDS

# AIM:

      To implement Dashboards creation with Plotly and Dash using python.
      

# About Dash and Plotly tools:

Dash is a Python framework for building analytical web applications. Dash helps in building responsive web dashboards that is good to look at and is very fast without the need to understand complex front-end frameworks or languages such as HTML, CSS, JavaScript. Let’s build our first web dashboard using Dash.

Plotly library in Python is an open-source library that can be used for data visualization and understanding data simply and easily. Plotly supports various types of plots like line charts, scatter plots, histograms, box plots, etc.


# ALGORITHM:

Step 1: Import Necessary Library like dash and plotly.

Step 2: Load the dataset.

Step 3: Add dropdown using layout function and include the necessary options.

Step 4: Display the necessary visualization tools and include the necessary parameters.

Step 5: Display the output.


# PROGRAM:
```
Developed By: Roselin mary jovita S
Register No : 212222230122
```


# CODING :
```
pip install dash plotly pandas
import dash
from dash import dcc, html
from dash.dependencies import Input,Output
import plotly.express as px
import pandas as pd
import plotly.graph_objects as px
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = sns.load_dataset('tips')
```

```
plot=px.Figure(data=[px.Scatter(x=df['day'],y=df['tip'],mode='markers')])
plot.update_layout(updatemenus=[dict(buttons=list([dict(args=["type","scatter"],label="Scatter Plot",method="restyle"),dict(args=["type","bar"],label="Bar Chart",method="restyle")]),direction="down",)])
plot.show()

```
```
import plotly.express as px
df=px.data.tips()fig = px.scatter_3d(df, x="total_bill",y="sex",z="tip",color='day',size='total_bill',symbol='time')
fig.show()
```

```
import plotly.express as px
df=px.data.tips()
fig = px.bar(df, x='day',y='total_bill',color='sex',facet_row='time',facet_col='sex')
fig.show()
```

```
import plotly.express as px
df=px.data.tips()
fig = px.histogram(df, x='total_bill',color='sex',nbins=50,histnorm='percent',barmode='overlay')
fig.show()
```

```
import plotly.express as px
df=px.data.tips()
fig = px.pie(df, values='total_bill',names='day')
fig.show()

```

# OUTPUT :

![Screenshot 2024-11-15 204715](https://github.com/user-attachments/assets/a4060c31-9547-4522-b020-d15d770ead90)

<table>
<tr>
<td>
      
![Screenshot 2024-11-15 204740](https://github.com/user-attachments/assets/80d5c19c-905e-4be1-9d15-737f3cb436ea)

</td>

<td>
      
![Screenshot 2024-11-15 204808](https://github.com/user-attachments/assets/d83bbe4f-9d11-4c9c-91c2-974d9050e750)

</td>
            
</tr>
</table>

![Screenshot 2024-11-15 204923](https://github.com/user-attachments/assets/79749ec0-cbc1-49a3-8f10-58f9c9ce768c)


![Screenshot 2024-11-15 204946](https://github.com/user-attachments/assets/4ac630ed-010a-4f96-a1ee-f0b1a454fdd3)


![Screenshot 2024-11-15 205005](https://github.com/user-attachments/assets/6163e4c6-c082-4d87-ab20-0379d3229314)

![Screenshot 2024-11-15 205053](https://github.com/user-attachments/assets/ee6cbf9f-d8d7-42e0-8f95-aad2e5fb76ed)

# RESULT:
Thus , To implement Dashboards creation with Plotly and Dash using python is successfully done.
