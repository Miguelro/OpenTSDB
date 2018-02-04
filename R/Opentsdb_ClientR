if(!require("stringr")) install.packages("stringr"); library("stringr")
if(!require("httr")) install.packages("httr"); library("httr")
if(!require("rjson")) install.packages("rjson"); library("rjson")
if(!require("lubridate")) install.packages("lubridate"); library("lubridate")
if(!require("data.table")) install.packages("data.table"); library("data.table")
if(!require("devtools")) install.packages("devtools"); library("devtools")
install_github("opentsdbr", "holstius")
library(opentsdbr)

start <- interval(ymd_hms("2017-11-28 16:00:00"),ymd_hms("2017-11-29 20:00:00"))

(result <- tsd_req(metric='open', interval=start, tags=c(symbol='GOOG',symbol='MSFT'),hostname = 'localhost', port=8091))
