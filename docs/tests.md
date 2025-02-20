# Ajout et exécution des tests pour le site

J'ai ajouté un script de test test.sh` pour vérifier que le site Docusaurus se construit correctement. Voici le contenu du script :

#!/bin/bash
npm run build
if [ $? -eq 0 ]; then
  echo "Build successful"
else
  echo "Build failed"
  exit 1
fi