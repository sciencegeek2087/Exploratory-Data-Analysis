install.packages("sqldf,descr", repos = "http://cran.cnr.berkeley.edu/")

read.csv.sqlf(https://d396qusza40orc.cloudfront.net/exdata%2Fdata%2Fhousehold_power_consumption.zip/household_power_consumption.txt, sql = 'select * from file' where Date = 1/2/2007 or Date = 2/2/2007, header = TRUE, sep = ";")

library(descr)
x = c("Global_active_power")
freq(x, plot = FALSE)

plot(FrequencyxGlobal_active_power[1,], Main = "Global Active Power", + xlab="Global active power (kilowatts)", ylab="Frequency", type="b", xaxt="n", axis(1,1:length
