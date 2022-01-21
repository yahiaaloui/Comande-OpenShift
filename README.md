# Comande-OpenShift
oc new-project mon_projet_avec_un_nom_unique pour débuter un projet
oc projects pour afficher mes projets
oc project mon_projet_avec_un_nom_unique pour entrer dans un projet
oc get templates -n openshift pour aficher les templates disponibles
oc process --parameters nom_du_template -n openshift pour afficher la documentation de chaque paramètre du template
oc new-app lamp pour déployer un projet avec les paramètre par défaut
oc new-app lamp -p PARM1=val_du_1er_param -p PARM2=val_du_1me_param etc. pour lancer une application paramétrée
oc get podspour afficher les Pods actifs du projet
oc rsh le_nom_du_pod pour se connecter dans un Pod actif
oc cp le_nom_du_pod:rep/fichier . ou oc cp fichier le_nom_du_pod:rep/ pour copier un fichier depuis/dans un Pod actif
oc rsync le_nom_du_pod:rep/fichier . ou oc rsync mon_dossier le_nom_du_pod:rep/ pour synchroniser un dossier depuis/dans un Pod actif
oc rollout latest dc/<name> pour redéployer une application
oc logs -f dc/<name> pour afficher le log d'un déploiment
oc logs --help aide de la commande logs
