data1 = data1[-5,]
names(data1)<-data1[-5,]
data1[-5,]
names(data1)<-c([-5,])


# -Data

# notion de vecteur
c(1,2,3,4)

c("a","b","c")

c("a",1,"c")

vecteur<- c("a","b","c")
vecteur2<- vecteur
vecteur3<- c(vecteur, vecteur2)



# Changer le type de données :
## base R
as.numeric(c('1','2','3'))
as.character(c(1,2,3))
as.factor(c(2,3,4))

# Attention pas de as.numeric directement sur un as.factor
as.factor(c(4,3,2))%>%as.character()%>%as.numeric()


data1$Sexe.du.medcin.traitant<-as.factor(data1$Sexe.du.medcin.traitant)
data1$Medecin.adresseur<- as.factor(data1$Medecin.adresseur)
