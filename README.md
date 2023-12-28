E-Bus est une simple application cmd , écrite en language C, assure la réservation d'un bus pour faire un voyage. 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
E-Bus est composé de deux espaces:
1.Espace Administration:
Ici l'application vous permet de voir et de modifier la liste des bus disponible : ajouter un bus, supprimer un bus en cas du panne et modifier le prix des bus disponible.
ce espace est même sécurisé par mot de passe (0000) .
2.Espace Client:
Ici notre chère client puisse sign in si il est nouveau ou bien tout simplement log in pour accéder à son compte ou son réservation.
Il peut soit créér un compte ,voir son compte, modifier son compte ou bien le supprimer.
De même pour la réservation soit réserver un bus ,modifier la réservation, voir la réservation ou la supprimer.
Pour plus des détails  voici ci dessous  les fonction utilisée dans la programation :
	int nbrlignes(FILE* f) :: return le nbr de lignes du fichier projetbus.txt
	int nbrlignes1(FILE* f) :: return le nbr de lignes du fichier listeactionprojetbus.txt
	int nbrlignes2(FILE* f) :: return le nbr de lignes du fichier modifierresprojetbus.txt
	int nbrlignes3(FILE* f) :: return le nbr de lignes du fichier administrateurprojetbus.txt
	void afficherdescriptionbus(FILE* f,int i) :: afficher la liste des bus disponible :: afficher le fichier projetbus.txt
	void afficheradministrateuraction(FILE* f,int i) :: afficher le fichier administrateurprojetbus.txt
	void afficherlisteaction(FILE* f,int i)   :: afficher le fichier listeactionprojetbus.txt
	void affichermodifresoption(FILE* f,int i)  :: afficher le fichier modifierresprojetbus.txt
	void administrateur(FILE* f,int nblignes) :: permet de présenter la liste des bus, ajouter un bus, supprimer un bus et modifier le prix des bus disponible.
	liste creationvoy(liste l) :: ajout tête d'un nouveau compte voyageur
	liste1 creationres(liste1 l1,int N) :: ajout tête d'une nouvelle reservation pour un compte voyageur  
	void affichagecompteres(liste1 l1) :: affichage les reservation des comptes du voyageur  
	void affichagecompteX(liste l) ::  affichage du compte du personne X
	void modifiercompteX(liste l) :: modifier compte du personne X
	void affichagereservationX(liste1 l1) ::  affichage du reservation du personne X
  void modifierres(liste1 l1) :: modifier du reservation du personne X
  void affichagestructbus(liste2 l2) :: affichage du structure bus
  void busdispo(int aux,liste2 l2,liste1 l1) :: affiche si la bus choisi est disponible au non
	liste1 supprimeres(liste1 l1)
