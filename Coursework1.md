install.packages("sqldf", repos = "http://cran.cnr.berkeley.edu/")

install.packages("descr", repos = "http://cran.cnr.berkeley.edu/")

install.packages("ggplot2", repos = "http://cran.cnr.berkeley.edu/")

selecteddata <- read.csv.sqlf(household_power_consumption.txt, sql = select * from file where Date = 1/2/2007 or Date = 2/2/2007, header = TRUE, sep = ";")

Global active power (kilowatts) <- c(selecteddata$Global_active_power)
hist(Global active power, col="red", ylim=c(0,1200))
dev.copy(png,filename="plot1.png");
dev.off ();

GAP <- data.frame(Date = factor(c("Thu", "Fri","Sat"), level=c("Thu", "Fri", "Sat")), Global_active_power=c(Global_active_power)
submetering1=c(Sub_metering_1)
submetering2=c(Sub_metering_2)
submetering3=c(Sub_metering_3)

library(ggplot2)

ggplot(data=GAP,aes(x=Date, y=Global_active_power, group=1) + geomline() + expand_limits(y=0) + ylab(Global Active Power (kilowatts)
dev.copy(png,filename="plot2.png");
dev.off ();

ggplot(data=GAP,aes(x=Date, y=submetering1,submetering2,submetering3 group=3 color=submetering1,submetering2,submetering3) + geomline() + expand_limits(y=0) + theme_bw() + theme(legend.position=c(.7, .4))
dev.copy(png,filename="plot3.png");
dev.off ();





# ALTERNATE METHOD for Plot1
# library(descr)
# x = c("Global_active_power")
# freq(x, plot = FALSE)
# plot(FrequencyxGlobal_active_power[1,], Main = "Global Active Power", + xlab="Global active power (kilowatts)", 
# ylab="Frequency", type="b", xaxt="n", axis(1,1:length
