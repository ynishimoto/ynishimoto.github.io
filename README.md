# Forecasting

```python
# *New* vendor to DDC data
folder = os.getcwd()
data_original_df = pd.read_csv(folder + '\\DDC710_inbound_agg_2020-11-01_2023-11-20.csv', parse_dates=['EVENT_DT'])\
    .sort_values('EVENT_DT')\
    .rename(columns={'EVENT_DT':'ds', 'QTY':'y'})

data_original_df.head()
```
