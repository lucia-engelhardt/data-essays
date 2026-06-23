# Chart Code

## Chart with Slider Chart Below It

import altair as alt
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import altair as alt
import pandas as pd

import altair as alt
alt.data_transformers.disable_max_rows()

ss = pd.read_csv('data/all-thumb.csv')
source = pd.DataFrame({'category': ['Boogie Nights', 'Hard Eight', 'Inherent Vice', 'Licorice Pizza', 'Magnolia', 'The Master', 'Phantom Thread', 'Punch-Drunk Love', 'There Will Be Blood'], 'value': 'seconds'})

categories = ['Boogie Nights', 'Hard Eight', 'Inherent Vice', 'Licorice Pizza', 'Magnolia', 'The Master', 'Phantom Thread', 'Punch-Drunk Love', 'There Will Be Blood']
color_mapping = ['#F47804', '#417505', '#7ED321', '#F5D323', '#52322C', '#2D5787', '#B65CE8', '#BF4983', '#A10215']

data = pd.read_csv('data/all-thumb.csv')

interval = alt.selection_interval(encodings=['x'])

base = alt.Chart(data).mark_tick(size=100, thickness=2).encode(
    x=alt.X('Seconds', axis=alt.Axis(titleFontSize=35)),
    y=alt.Y('Film', axis=alt.Axis(titleFontSize=35)),
    color=alt.Color(
        'Film', 
        scale=alt.Scale(domain=categories, range=color_mapping))
)

chart1 = base.encode(
    x=alt.X('Seconds', axis=alt.Axis(titleFontSize=35, labelFontSize=30), scale=alt.Scale(domain=interval.ref())), 
    y=alt.Y('Film', axis=alt.Axis(titleFontSize=35, labelFontSize=30)),
    tooltip=['image']
).properties(
    width=1500,
    height=900,
)

chart2 = base.add_selection(
    interval
).mark_tick(size=10, thickness=2
).properties(
    width=1500,
    height=300,
)

chart & view
