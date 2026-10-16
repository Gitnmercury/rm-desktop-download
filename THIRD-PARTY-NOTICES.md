# Composants tiers

rM Desktop appartient à Anthony BELKACEM EI (voir LICENSE.md). Il s'appuie sur les composants
suivants, qui restent la propriété de leurs détenteurs et soumis à leurs propres licences.

## Application Windows (C# / WPF)

| Composant | Propriétaire | Licence |
|---|---|---|
| .NET 8, WPF | Microsoft / .NET Foundation | MIT |
| Windows SDK Projections, CsWinRT | Microsoft | MIT |
| OpenSSH (ssh, ssh-keygen) | Projet OpenSSH (OpenBSD) ; portage Windows : Microsoft (Win32-OpenSSH) | BSD |
| Windows.Data.Pdf, Windows.Media.Ocr | Microsoft | Composants Windows |
| DPAPI, AES-GCM, PBKDF2 | Microsoft (.NET / Windows) | MIT / Windows |
| Segoe Fluent Icons, Segoe MDL2 Assets | Microsoft | Fournies avec Windows, non redistribuables |
| Microsoft Word (optionnel, conversion Word vers PDF) | Microsoft | Licence de l'utilisateur, non fourni |
| Claude Code (outil de développement, non livré) | Anthropic | Hors logiciel livré |

## Version Python

| Composant | Propriétaire | Licence |
|---|---|---|
| Python, Tkinter (Tcl/Tk) | Python Software Foundation ; Tcl Core Team | PSF ; BSD |
| OpenSSH (ssh, ssh-keygen) | Projet OpenSSH (OpenBSD) ; portage Windows : Microsoft (Win32-OpenSSH) | BSD |
| Pillow (optionnel) | Jeffrey A. Clark et contributeurs | MIT-CMU (HPND) |
| PyMuPDF (optionnel, à installer soi-même) | Artifex Software | AGPL-3.0 |
| Windows.Media.Ocr (OCR sous Windows) | Microsoft | Composant Windows |
| Tesseract (OCR sous Linux, optionnel) | Projet Tesseract | Apache 2.0 |
| LibreOffice (optionnel, conversion Word sous Linux) | The Document Foundation | MPL 2.0 |
| Segoe Fluent Icons, Segoe MDL2 Assets | Microsoft | Fournies avec Windows, non redistribuables |
| DejaVu (icônes sous Linux) | Projet DejaVu | Licence libre DejaVu (Bitstream Vera) |
| Claude Code (outil de développement, non livré) | Anthropic | Hors logiciel livré |

PyMuPDF est sous licence AGPL-3.0 : il n'est jamais fourni avec le logiciel. L'utilisateur qui
l'installe le fait sous sa propre responsabilité.

Les marques et icônes tierces restent la propriété de leurs détenteurs.

## Ressources graphiques

Les éléments graphiques de rM Desktop n'ont pas tous la même origine ni le même statut. Cette
section les distingue. Elle informe, mais ne constitue ni une licence ni une autorisation de
redistribuer un élément appartenant à un tiers.

### Visuels réalisés à l'aide d'outils d'intelligence artificielle

| Fichier | Outil utilisé | Usage dans le logiciel |
|---|---|---|
| `src/rem_1.jpg` | Service d'IA de Google (Gemini) | Écran de démarrage et « Fiche tablette » : reMarkable 1 détectée |
| `src/rem_2.jpg` | Service d'IA de Google (Gemini) | Écran de démarrage et « Fiche tablette » : reMarkable 2 détectée |
| `src/no_rem.jpg` | Service d'IA de Google (Gemini) | Écran de démarrage et « Fiche tablette » : modèle non reconnu |
| `src/usb-c-out-16-9.jpg` | Service d'IA de Google (Gemini) | Carte « Tablette déconnectée » |
| `src/Sleepingmod16-9.jpg` | Service d'IA de Google (Gemini) | Mode veille de l'application |
| `src/screensaver_desktop.png` | Service d'IA d'OpenAI | Image proposée pour l'écran de veille de la tablette |

Ces visuels ont été réalisés dans le cadre d'une prestation payée, à partir d'instructions rédigées
par l'auteur, qui les a ensuite sélectionnés et/ou retouchés. L'outil n'est pas présenté comme
leur auteur. Les droits que l'auteur peut revendiquer dépendent de la part de sa contribution
créative : une image générée n'est pas automatiquement protégée par le droit d'auteur, et le
paiement d'un service ne vaut pas, à lui seul, cession de droits. Leur utilisation reste soumise
aux conditions des services concernés et aux droits éventuels de tiers.

Les métadonnées de provenance (C2PA) ont été retirées des fichiers livrés pour des raisons de
confidentialité. Cette section indique leur origine à la place. Les images produites par Google
peuvent aussi contenir un filigrane invisible (SynthID), qui fait partie de l'image elle-même.

`rem_1.jpg`, `rem_2.jpg` et `no_rem.jpg` représentent des tablettes et des stylets semblables aux
produits reMarkable, pour aider l'utilisateur à reconnaître son appareil. Les inscriptions et logos
visibles ont été retirés par retouche. L'apparence des produits, les noms et les marques reMarkable
appartiennent à reMarkable AS ; leur évocation ne signifie pas que reMarkable soutient ou approuve
rM Desktop.

### Autres éléments graphiques

| Élément | Origine |
|---|---|
| `src/rM_Desktop.png`, `src/rM_Desktop*.ico` (icône de l'application) | Créés ou modifiés pour le projet par l'auteur |
| Icônes de l'interface | Polices Segoe Fluent Icons / MDL2 (Microsoft, fournies avec Windows, non livrées) ; DejaVu sous Linux |
