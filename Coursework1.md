install.packages("sqldf", repos = "http://cran.cnr.berkeley.edu/")

read.csv.sqlf(https://d396qusza40orc.cloudfront.net/exdata%2Fdata%2Fhousehold_power_consumption.zip/household_power_consumption.txt, sql = "select * from file", header = TRUE, sep = ";", filter =
