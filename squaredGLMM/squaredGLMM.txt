# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Pseudo-R-squared for Generalized Mixed-Effect models Use squaredGLMM (MuMIn) With (In) R Software
install.packages("MuMIn")
library("MuMIn")
library("nlme")
squaredGLMM = read.csv("https://raw.githubusercontent.com/timbulwidodostp/squaredGLMM/main/squaredGLMM/squaredGLMM.csv",sep = ";")
# Estimation Pseudo-R-squared for Generalized Mixed-Effect models Use squaredGLMM (MuMIn) With (In) R Software
lme <- lme(distance ~ Sex * age, ~ 1 | Subject, data = squaredGLMM)
r.squaredGLMM(lme)
r.squaredLR(lme)
r.squaredLR(lme, null.RE = TRUE)
# Pseudo-R-squared for Generalized Mixed-Effect models Use squaredGLMM (MuMIn) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished