SELECTED DESCRIPTIVE AND INFERENTIAL STATISTICS IN R FOR UNDERGRADUATE PROJECT

BEING A PRACTICAL AND DEMONSTRATION SESSSION HELD ON THURSDAY, 18TH MAY, 2023 AT STATISTICS DEPARTMENT, THE FEDERAL POLYTECHNIC OFFA

BY
DR. ABDULKABIR MURITALA
# Descriptives Statistics simulation
x=rnorm(100)
mean(x)
var(x)
sd(x)
median(x)
summary(x)
barplot(x)
hist(x)
qqnorm(x)
boxplot(x)
dotchart(x)

#Real life data
x=c(1,3,5,6,7,8,9,3,2,4)
y=c(2,3,5,6,7,8,4,3,2,1)
z=c(2,3,4,1,2,5,6,7,8,9)
boxplot(x,y,z)
boxplot(x,y,z,horizontal=T)
boxplot(x,y,z,horizontal=T,names=c("A","B","C"))
boxplot(x,y,z,horizontal=T,names=c("A","B","C"),col=c("red","black","blue"))
par(mfrow=c(2,2))
barplot(x,y,z)
hist(x)

# Inferential Statistics
# chi sqaure
data <- matrix(c(100, 70, 20, 90, 75, 25), ncol=3, byrow=TRUE)
colnames(data) <- c("Rep","Dem","Ind")
rownames(data) <- c("Male","Female")
data <- as.table(data)
data
chisq.test(data)
# one sample t.test
daily.sales=c(5260,5470,5640,6180,6390,6515,6805,7515,7515,8230,8770)
mean(daily.sales)
sd(daily.sales)
quantile(daily.sales)
t.test(daily.sales)
t.test(daily.sales,mu=7000)

# Two sample
dat=read.csv("hnd.csv")
View(dat)
attach(dat)
dat
t.test(student~sex)
t.test(exp~time,var.equal=T
var.test(exp~time,var.equal=T)
# Paired sample t-test
t.test(pre,post,paired=T)

# Regression
x1=runif(50,2,3)
x2=rnorm(50,4,1)
y=2*x1+x2
dat=data.frame(y,x1,x2)
reg=lm(y~x1+x2,dat)
summary(reg)
plot(y,x1)
abline(lm(y~x1))
predict(reg)
anova(lm(y~x1))

# correlation 
x1=rnorm(100,2,1)
x2=rnorm(100,2,4)
cor.test(x1,x2)
cor.test(x1,x2,method="spearman")
cor.test(x1,x2,method="kendall")
# One way ANOVA
x1=runif(50,2,3)
y=2*x1+x2
anova(lm(y~x1))

# two way ANOVA
heart.rate=data.frame(hr=c(96,110,89,95,128,100,72,79,100,
                                92,106,86,78,124, 98,68,75,106,
                                86,108,85,78,118,100,67,74,104,
                                92,114,83,83,118,94,71,74,102),
                         subj=gl(9,1,36),
                         time=gl(4,9,36,labels=c(0,30,60,120)))
anova(lm(hr~subj+time))
gl(9,1,36)
gl(4,9,36,labels=c(0,30,60,120))

# Two way Anova
x1=runif(50,2,3)
x2=rnorm(50,4,1)
y=2*x1+x2
dat=data.frame(y,x1,x2)
reg=lm(y~x1+x2,dat)
anova(lm(y~x1+x2,dat))


# Two way Anova with replication
x1=runif(50,2,3)
x2=rnorm(50,4,1)
y=2*x1+x2
dat=data.frame(y,x1,x2)
reg=lm(y~x1*x2,dat)
anova(lm(y~x1*x2,dat))

# Time series
Infla=ts(c(13.8,15.7,3.2,5.4,13.2,34.4,23.7,15.6,16.6),start= c(1970,1))
plot(Infla)
acf(Infla)
pacf(Infla)
library(tseries)
adf.test(Infla)
adf.test(diff(Infla))

# Moving average 
InflaSMA2<-SMA(Infla, n=2)
InflaSMA2
plot(InflaSMA2)
dat=read.csv("kay.csv")
dat2=write.csv(dat,"jm.csv")

YOU ALL HAVE DONE WONDERFULLY WELL
IT HAS BEEN NICE BEING WITH YOU
KEEP IT UP
