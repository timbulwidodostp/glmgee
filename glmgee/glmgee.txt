# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fit generalized estimating equations Use glmgee (glmtoolbox) With (In) R Software
install.packages("glmtoolbox")
library("glmtoolbox")
glmgee = read.csv("https://raw.githubusercontent.com/timbulwidodostp/glmgee/main/glmgee/glmgee.csv",sep = ";")
# Estimation Fit generalized estimating equations Use glmgee (glmtoolbox) With (In) R Software
glmgee_1 <- Dependen ~ poly(Independen_1,4) + Independen_2
glmgee_2 <- glmgee(glmgee_1, id=Id, family=Gamma(log), corstr="AR-M-dependent(1)", data=glmgee)
summary(glmgee_2, corr.digits=2)
# Fit generalized estimating equations Use glmgee (glmtoolbox) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished