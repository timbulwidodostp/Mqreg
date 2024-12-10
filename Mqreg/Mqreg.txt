# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Semiparametric M-Quantile Regression Use Mqreg (expectreg) With (In) R Software
install.packages("expectreg")
install.packages("SemiPar")
library("expectreg")
Mqreg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/Mqreg/main/Mqreg/Mqreg.csv",sep = ";")
Mqreg <- Mqreg(logratio~rb(range,"pspline"),data=Mqreg,smooth="f", tau=c(0.05,0.5,0.95),lambda=10)
Mqreg
plot(Mqreg,rug=FALSE)
# Semiparametric M-Quantile Regression Use Mqreg (expectreg) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished