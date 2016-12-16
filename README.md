# Rendu du projet SmallUML

Cette archive contient le code source du projet SmallUML du groupe de Léo Cassiau et Geoffrey Desbrosses.
Vous y trouverez les fichiers suivants :

- smallUML/SmallUML/model/smalluml.ecore : le méta-modèle SmallUML
- org.smalluml.SmallUML/src/org/smalluml/SmallUML.xtext : la grammaire du méta-modèle SmallUML défini dans smalluml.ecore
- SmallToUML/src/Small2UML.atl : les règles ATL de transformations d'un modèle en SmallUML vers un modèle en UML.
- SmallToUML/inModels/SmallUMLParking.xmi : un modèle simple respectant notre méta-modèle SmallUML représentant un parking.
- SmallToUML/outModels/UMLParking.xmi : le résultat de la transformation de SmallUMLParking.xmi à l'aide de Small2UML.atl.
- SmallToUML/launchConfiguration/Small2UML.launch : configuration de la transformation ATL du modèle de parking.

Pour réaliser la transformation vous devez :

- importer ce dossier sous eclipse.
- générer le code correspondant au fichier smalluml.ecore. Pour cela, dans le fichier smalluml.genmodel, faites un clique droit à la racine et utilisé l'option "Generate Model Code"
- 
