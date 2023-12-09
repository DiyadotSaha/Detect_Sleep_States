# CS 184A/284A - AI in Biology and Medicine
## Diya Saha (sahad1@uci.edu) | Abhinand Ganesh (aganesh5@uci.edu)

### Because of Github's size requirements, data has been provided for the following `series_id` : `['1b92be89db4c', '655f19eabf1e', '5c55a5e717d6']`

## Two sets of data stores are made available 
  <ul>
    <li> data/train_events_csv.csv </li>
    <li> data/pandas_df.csv </li>
  </ul>

## The following libraries are needed
<ul>
  <li> TensorFlow </li>
  <li> pandas </li>
  <li> numpy </li>
  <li> matplotlib </li>
  <li> sklearn </li>
</ul>

## How to import datasets
`train_events_csv = pd.read_csv('/data/train_events.csv')`
<br>
`pandas_df = pd.read_csv('/data/pandas_df.csv')`

## Run feature expansion code
`randomseries= ['1b92be89db4c', '655f19eabf1e', '5c55a5e717d6']`
<br>
`feature_df=merging_patients(randomseries)`
