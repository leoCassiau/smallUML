# Rendu du projet SmallUML

Cette archive contient le code source du projet SmallUML du groupe de Léo Cassiau et Geoffrey Desbrosses.
Vous y trouverez les fichiers suivants :

- smallUML/SmallUML/model/smalluml.ecore : le méta-modèle SmallUML.
- org.smalluml.SmallUML/src/org/smalluml/SmallUML.xtext : la grammaire du méta-modèle SmallUML défini dans smalluml.ecore.
- org.smalluml.SmallUML/examples/parking.suml : exemple de modèle de parking respectant la grammaire de SmallUML.xtext 
- SmallToUML/src/Small2UML.atl : les règles ATL de transformations d'un modèle en SmallUML vers un modèle en UML.
- SmallToUML/inModels/SmallUMLParking.xmi : un modèle de parking simple respectant notre méta-modèle SmallUML représentant un parking.
- SmallToUML/outModels/UMLParking.xmi : le résultat de la transformation de SmallUMLParking.xmi à l'aide de Small2UML.atl.
- SmallToUML/launchConfiguration/Small2UML.launch : configuration de la transformation ATL du modèle de parking.

## Installation
Pour réaliser la transformation et utiliser la grammaire vous devez au préalable :

- posséder une version d'eclipse avec ATL, EMF et Xtext d'installé.
- importer ce dossier sous eclipse.
- dans le projet SmallUML : générez le code correspondant au fichier smalluml.ecore. Pour cela, dans le fichier smalluml.genmodel, faites un clique droit à la racine et utilisez l'option "Generate Model Code".
- dans le projet org.smalluml.SmallUML : générez le code nécessaire pour utiliser la grammaire Xtext de SmallUML. Pour cela, lancé le fichier SmallUML.xtext (Generate Xtext Artifacts).

## Utilisation
Pour écrire une modèle avec la grammaire Xtext : clique droit sur le projet org.smalluml.SmallUML > Run as... > Eclipse Application. Vous devez alors créer une projet simple, ajouter un fichier d'extension .suml dans ce projet. Eclipse va alors demander de changer la nature du projet, confirmez, et vous pouvez maintenant rédiger un modèle respectant le méta-modèle de SmallUML.

Pour transformer un modèle, lancez simplement le fichier Small2UML.atl avec la configuration défini dans le fichier Small2UML.launch.
