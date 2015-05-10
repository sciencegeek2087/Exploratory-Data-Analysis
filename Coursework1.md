install.packages("sqldf,descr,ggplot2", repos = "http://cran.cnr.berkeley.edu/")

selected_data <- read.csv.sqlf(https://d396qusza40orc.cloudfront.net/exdata%2Fdata%2Fhousehold_power_consumption.zip/household_power_consumption.txt, sql = 'select * from file' where Date = 1/2/2007 or Date = 2/2/2007, header = TRUE, sep = ";")

Global active power (kilowatts) <- c(selected_data$Global_active_power)
hist(Global active power, col="red", ylim=c(0,1200))
dev.copy(png,filename="plot1.png");
dev.off ();

# ALTERNATE METHOD for Plot1
# library(descr)
# x = c("Global_active_power")
# freq(x, plot = FALSE)
# plot(FrequencyxGlobal_active_power[1,], Main = "Global Active Power", + xlab="Global active power (kilowatts)", 
# ylab="Frequency", type="b", xaxt="n", axis(1,1:length


GAP <- data.frame(Date = factor(c("Thu", "Fri","Sat"), level=c("Thu", "Fri", "Sat")), Global_active_power=c(Global_active_power)
Sub metering 1=c(Sub_metering_1)
Sub metering 2=c(Sub_metering_2)
Sub metering 3=c(Sub_metering_3)

library(ggplot2)

ggplot(data=GAP,aes(x=Date, y=Global_active_power, group=1) + geomline() + expand_limits(y=0) + ylab(Global Active Power (kilowatts)
dev.copy(png,filename="plot2.png");
dev.off ();

ggplot(data=GAP,aes(x=Date, y=
