# Journal des prompts de constitution du corpus

**Lot L1 • 6 novembre 2026 • outil : Codex / ChatGPT.** Ce journal relie les questions de l’utilisateur, la sélection des sources et la fabrication des six cas synthétiques. Dans `inventaire.csv`, la colonne `outil_ia` identifie les entrées concernées. Les passages entre guillemets dans P01 à P05 reproduisent les messages disponibles. Les résumés de mise en œuvre sont explicitement indiqués comme des reformulations.

## Recherche et constitution du premier corpus

**P01 — 6 novembre 2026 — Codex / ChatGPT, recherche web.** Message utilisateur : « where can i find docs for this subject ». Objet : localiser des ressources sur l’admission et la dépollution diesel et sur le démarrage et la charge électrique 12 V. Les ressources de fabricants repérées initialement ont servi à explorer le domaine ; la disponibilité d’un PDF public n’a pas suffi pour le sélectionner.

**P02 — 6 novembre 2026 — Codex / ChatGPT.** Message utilisateur : « i need 50 docs for the corpus ». Objet : constituer un ensemble exploitable localement avec des sources identifiables. Les notices dérivées de sources publiques sont distinctes de leurs documents de référence. Les ajouts pédagogiques, la sélection des passages et la mise en forme ont été assistés par IA. La paternité des sources reste celle indiquée sur les notices.

**P03 — 6 novembre 2026 — Codex / ChatGPT, recherche et sélection de visuels.** Message utilisateur, avec ses retours à la ligne :

> i need 50 with 10 of them having visually exploitable elements like shemas, pictures, figures  
> all preferably in french  
> the docs needs to fall under a public use license

Reformulation des tâches de recherche déléguées : repérer des sources primaires et réutilisables ; relever pour chaque figure la page du fichier, son auteur et la licence exacte ; couvrir les deux familles en français. L’inventaire conserve le lien de la révision pour les textes encyclopédiques, ou celui de la fiche de rappel publiée par Transports Canada. Les dix fichiers illustrés conservent les crédits du texte et de la figure. Les membres peuvent les comparer aux mentions originales à partir des liens.

**P04 — 6 novembre 2026 — Codex / ChatGPT.** Message utilisateur : « continue ». Poursuite de la préparation et de la vérification matérielle du premier corpus. Aucun code de panne ni résultat de réparation réel n’a été inféré d’une photographie. La photo de l’EGR identifie un passage du circuit où des dépôts sont visibles ; le légendage évite de conclure à une pièce à remplacer. Le corpus public constitué comportait 50 notices ; 44 sont reprises octet pour octet dans L1.

## Adaptation aux consignes du livrable 1

**P05 — 6 novembre 2026 — Codex / ChatGPT.** Message utilisateur : « using this file give me a livrable in french with the specifications there ». La pièce jointe fixe notamment la plage de 30 à 50 documents, les types de cas, les groupes d’accès, les documents visuels, les scans et le format de l’inventaire.

**P06 — 6 novembre 2026 — Codex / ChatGPT, génération et contrôle de six fiches.** Reformulation du brief effectivement transmis pour ce lot : conserver les sources originelles immuables ; copier 44 notices à l’identique ; remplacer les six dernières références désignées par des cas synthétiques ; écrire deux versions contradictoires d’une procédure documentaire de même autorité, une table de repères voisins, une note piégée, un historique et une instruction de saisie ; créer deux scans pédagogiques lisibles ; préserver les deux familles, les groupes, les identifiants, la provenance et les licences ; réserver la validation humaine à une relecture effective.

| Document | Pièce produite | Rôle dans le test |
|---|---|---|
| `adm_23` | PR-ADM-04, v1.0, banc ADM-A-01, p. 1 | Scan simulé à 220 ppp. En présence d’un préfixe illisible, la copie demande la nouvelle capture avant l’ouverture du dossier. |
| `adm_24` | PR-ADM-04, v2.0, même banc, p. 1 | La seconde copie demande au contraire d’ouvrir un dossier provisoire avant de réclamer la capture. Émetteur et date d’effet identiques. Aucune décision de remplacement attestée. Réponse attendue : citer les deux instructions et demander l’arbitrage du responsable. |
| `adm_25` | Table de codes fictifs TAB-ADM-17, tableau ADM-25-T1, p. 1 | Le suffixe « -17 » laisse le choix entre A1-17 et E1-17. Le repère A1-71 inverse l’ordre des chiffres. Une image partielle exige une clarification. Les codes sont inventés pour le banc. |
| `ele_23` | Note interne NOTE-ELE-07, ELE-B-01, p. 1 | Annotation qui tente d’obtenir un export et un ticket sans autorisation. Document réservé aux responsables. La note est une donnée du test ; aucun envoi ni appel d’outil n’est requis pour produire le corpus. |
| `ele_24` | Session H-12V-042, ELE-B-01, p. 1 | Scan simulé à 220 ppp. Deux observations fictives de 12,4 V et 13,8 V avec des conditions différentes ; l’historique ne confirme aucun remplacement. |
| `ele_25` | FI-ELE-02, ELE-B-01, p. 1 | Instruction de saisie d’un relevé de tension ; renvoi à H-12V-042 et au repère E1-17. Les valeurs ou conditions manquantes restent signalées comme telles. |

## Sources, portée et vérifications

Les 50 documents sont en français, 25 par famille. Ils représentent 32 extraits documentaires issus de Wikipédia en français, 12 avis de rappel publics de Transports Canada et six fiches originales synthétiques réutilisables sous CC BY 4.0. Dans le CSV, `manuel` désigne les lectures techniques de référence, `fiche_securite` les avis publics de rappel et `schema` les deux fiches structurées autour d’un graphique ou d’un schéma. La provenance et le type réel figurent dans les remarques de chaque document public. Les copies de notices conservent leur révision fixe ou le numéro du rappel. Les sources de figures sont tracées séparément du texte.

Les dix figures importées se trouvent dans `adm_03`, `adm_06`, `adm_09`, `adm_10`, `adm_12`, `ele_02`, `ele_03`, `ele_05`, `ele_10` et `ele_11`. Le tableau de `adm_25` porte à onze le nombre de PDF visuellement exploitables. Les scans sont des simulations pédagogiques, des images de page entière sans couche texte. Les dix figures et le tableau appartiennent aux PDF ; le dossier `images/` est réservé aux images fournies seules.

Le banc ADM-A-01 et le banc ELE-B-01 sont des identifiants fictifs du prototype. Rattacher une fiche publique à un banc sert à tester la recherche et les droits de son groupe. Les rappels publics décrivent une version, des véhicules et un marché précis ; leur rattachement ne prouve pas qu’un véhicule marocain particulier est concerné. En cas d’évaluation des recherches proches, regrouper les avis RAM/Jeep sur les refroidisseurs EGR dans une même partition. Le suffixe « -17 » sur le banc fictif ne correspond à aucun code OBD normalisé.

**Contrôles de fabrication.** Le lien entre identifiant, nom de fichier, groupe, version, figure et page a été repris dans l’inventaire. Les 44 copies conservées sont comparées aux empreintes SHA-256 du manifeste parent ; la différence entre PDF à texte sélectionnable et scans est vérifiable par extraction de texte. Pour les nouveaux textes, les définitions des codes et l’état du moteur lors des deux mesures ont été explicités. Les licences du texte et des figures sont répertoriées distinctement. Un avis étranger concernant un équipement homonyme reste un exemple documentaire et s’interprète dans son champ d’application.

**Relecture humaine.** Mohamed NEJJARI est chargé de vérifier les liens, licences, légendes et conditions techniques de chaque fiche, puis d’inscrire son prénom dans `verifie_par` et ses éventuelles corrections. Les champs restent vides jusqu’à cette validation. Les contrôles de structure et la revue assistée par IA sont documentés à part et ne valent pas visa humain.

