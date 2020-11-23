# Event Study Tool
Takes stock tickers, window parameters, and a date as inputs. Ouputs an event study. Cell 8 calls the openstock function. It takes the following parameters:

* stock_tickers: a list of strings, represents the stocks to be studied.
  * ['C', 'JPM']
* etf_ticker: a single string, represents etf (currently obsolete, enter empty string):
  * 'EFC'
* event_date: a date (dd-mm-yyyy), represents the event date you want to study:
  * '31-12-2020'
* est_window_size: integer, represents the size of the estimation window:
  * 100
* event_lead: integer, represents the size of the window before (and not including) the event date:
  * 3
* event_lag: integer, represents the size of the window after (and not including) the event date:
  * 3

Output shows the sensitivity of the firm to the event occuring on the event date. Statistical significance occurs at t-stat > 2.75.

**Note: Due to GitHub limitations, available stock data is limited to the first 99. Download the full dataset at Kaggle.**
