Guanhua Wang - Mingqiang WANG

/******** ATTENTION ***********/
La page index du projet est en xml et se situe dans le dossier "html" du "web" avec son xslt. Cette organisation est pour la raison d'affichage dans le navigateur du html transformé depuis xml. Vous ouvrez le fichier index.xml dans un navigateur Firefox(ou d'autres compatibles) et l'affichage est en html.
/******************************/

/data
	/CSV
	- fontaines-a-boire.csv : information des fontaine à boire à Paris (source https://opendata.paris.fr).
	- parcsetjardinsparis2010.csv : information des espaces verts parisiens avec géolocalisation (source https://opendata.paris.fr) 
	- zones-touristiques-internationales.csv : information des zones touristiques parisiens avec géolocalisation (source https://opendata.paris.fr) 

	/XML
	- fontaines-a-boire.xml : information des fontaine à boire à Paris (tranformé de csv).
	- parcsetjardinsparis2010.xml : information des espaces verts parisiens avec géolocalisation (tranformé de csv) 
	- zones-touristiques-internationales.xml : information des zones touristiques parisiens avec géolocalisation (tranformé de csv) 

	/JSON
	- parcsetjardinsparis2010.geojson : géocoordonnées des espaces verts parisiens (source https://opendata.paris.fr).
	- zones-touristiques-internationales.geojson : géocoordonnées des des zones touristiques parisiens (source https://opendata.paris.fr).

/grammaire
	* : Grammaires de validation sous forme dtd et rng pour les documents xml.

/script
	- csv2xml_espacevert.py : prétaitement et modélisation des données espaces verts en xml.
	- csv2xml_fontaine.py : prétaitement et modélisation des données fontaines en xml.	
	- csv2xml_zonetouristiques.py : modélisation des données zones touristiques en xml.
	- xml2html_arron.py : construction du tableau de fontaines selon arrondissement.
	- xml2html_modele.py : construction du tableau de fontaines potables selon modèle.		
	- xml2html_espacevert.py : construction du tableau des espaces verts.
	- xml2html_zonetouristique.py : construction du tableau des zone touristiques.
	- Projet_carte_Geojson.py : projection des fontaines, des espaces verts, des zones touristiques dans une carte OpenStreetMap.
	- carte_nombrefontaines.py :  projection des fontaines en groupant des marqueurs dans une carte Google.

/transformation
	- fontaines-a-boire.xsl : construction du tableau de fontaines.


/web
	* : Site web.


/xml
	- parcsetjardinsparis2010.xml : information des espaces verts parisiens avec géolocalisation (tranformé de csv) 
	- zones-touristiques-internationales.xml : information des zones touristiques parisiens avec géolocalisation (tranformé de csv) 
	- index.xml : contruction de notre site principal.
