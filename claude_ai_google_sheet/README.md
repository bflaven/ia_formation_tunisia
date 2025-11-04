# claude_ai_google_sheet.md

## FICHIERS
Il existe deux fichiers : 
- test_claude_tunisia.xlsx
- test_claude_tunisia_playlist.xlsx


## RESSOURCES

- ETAPE_1 - Vous allez devoir installer cette l'extension Chrome "Claude for Sheets" dont vous allez avoir besoin pour connecter avec l'API Claude et vos tableurs Excel sur google docs. Voir https://workspace.google.com/marketplace/app/claude%5Ffor%5Fsheets/909417792257

- ETAPE_2 - Vous allez devoir obtenir une clé d'API sur claude à cette adresse. Voir https://console.anthropic.com/



- ETAPE_3 - Voilà la documention officiel pour "jouer" avec l'extension Chrome "Claude for Sheets" et vos google docs. Voir https://docs.anthropic.com/en/docs/agents-and-tools/claude-for-sheets


**Ci-dessous des explications en français pour faire étape par étape l'installation et l'utilisation de l'extension Chrome "Claude for Sheets"**


## Claude for Sheets

## Présentation
Claude for Sheets est une extension qui intègre Claude, l'assistant IA d'Anthropic, directement dans Google Sheets. Cette intégration vous permet d'exécuter des interactions avec Claude directement dans les cellules de vos feuilles de calcul.

## Pourquoi utiliser Claude for Sheets ?
- **Ingénierie de prompts à grande échelle** - Testez vos prompts sur des suites d'évaluation en parallèle
- **Analyse de sondages** - Facilitez l'analyse de données d'enquêtes
- **Traitement de données en ligne** - Automatisez le traitement des données web
- **Tâches bureautiques** - Optimisez vos workflows administratifs

## Installation

### 1. Obtenir une clé API Anthropic
Si vous n'avez pas encore de clé API, vous pouvez en créer une dans la [Console Anthropic](https://console.anthropic.com/settings/keys).

### 2. Installer l'extension Claude for Sheets
Trouvez l'[extension Claude for Sheets](https://workspace.google.com/marketplace/app/claude%5Ffor%5Fsheets/909417792257) dans le marketplace des add-ons, puis cliquez sur le bouton bleu "Installer" et acceptez les permissions.

### 3. Connecter votre clé API
Entrez votre clé API en suivant ce chemin :
Extensions > Claude for Sheets™ > Open sidebar > ☰ > Settings > API provider

**Note importante :** Vous devrez saisir à nouveau votre clé API chaque fois que vous créerez une nouvelle feuille Google Sheet.

## Utilisation de base

### Fonction CLAUDE()
Pour votre premier prompt, utilisez la fonction CLAUDE() :

```
=CLAUDE("Claude, en une phrase, qu'est-ce qui est bien avec la couleur bleue ?")
```

Claude répondra avec une réponse. Vous saurez que le prompt est en cours de traitement car la cellule affichera "Loading...".

### Ajout de paramètres
Les arguments de paramètres viennent après le prompt initial :

```
=CLAUDE(prompt, modèle, params...)
```

Le modèle est toujours le deuxième élément de la liste. Exemple :

```
=CLAUDE("Bonjour, Claude !", "claude-3-haiku-20240307", "max_tokens", 3)
```

N'importe quel [paramètre API](/en/api/messages) peut être défini de cette façon. Vous pouvez même passer une clé API à utiliser uniquement pour cette cellule spécifique :

```
"api_key", "sk-ant-api03-j1W..."
```

## Utilisation avancée

### CLAUDEMESSAGES
La fonction CLAUDEMESSAGES vous permet d'utiliser spécifiquement l'[API Messages](/en/api/messages). Cela vous permet d'envoyer une série de messages "User:" et "Assistant:" à Claude.

C'est particulièrement utile si vous souhaitez simuler une conversation ou [préremplir la réponse de Claude](/en/docs/build-with-claude/prompt-engineering/prefill-claudes-response).

### Sauts de ligne
Chaque tour de conversation suivant (User: ou Assistant:) doit être précédé d'un seul saut de ligne. Pour entrer des sauts de ligne dans une cellule, utilisez les combinaisons de touches suivantes :
- Mac : Cmd + Entrée
- Windows : Alt + Entrée

### Paramètres facultatifs
Vous pouvez spécifier des paramètres API facultatifs en listant des paires argument-valeur. Vous pouvez définir plusieurs paramètres. Listez-les simplement l'un après l'autre, chaque paire argument-valeur étant séparée par des virgules.

Les deux premiers paramètres doivent toujours être le prompt et le modèle. Vous ne pouvez pas définir un paramètre facultatif sans également définir le modèle.

#### Principaux paramètres :

| Argument | Description |
|----------|-------------|
| max_tokens | Le nombre total de tokens que le modèle produit avant d'être forcé de s'arrêter. Pour les réponses oui/non ou à choix multiples, vous pouvez définir la valeur entre 1 et 3. |
| temperature | La quantité d'aléatoire injectée dans les résultats. Pour les tâches à choix multiples ou analytiques, vous la voudrez proche de 0. Pour la génération d'idées, vous la voudrez à 1. |
| system | Utilisé pour spécifier un prompt système, qui peut fournir des détails de rôle et du contexte à Claude. |
| stop_sequences | Tableau JSON de chaînes qui amèneront le modèle à arrêter de générer du texte si elles sont rencontrées. En raison des règles d'échappement dans Google Sheets™, les guillemets doubles à l'intérieur de la chaîne doivent être échappés en les doublant. |
| api_key | Utilisé pour spécifier une clé API particulière avec laquelle appeler Claude. |

## Exemples d'utilisation

### Tutoriel interactif d'ingénierie de prompts
Notre [tutoriel interactif approfondi d'ingénierie de prompts](https://docs.google.com/spreadsheets/d/19jzLgRruG9kjUQNKtCg1ZjdD6l6weA6qRXG5zLIAhC8/edit?usp=sharing) utilise Claude for Sheets. Consultez-le pour apprendre ou vous rafraîchir sur les techniques d'ingénierie de prompts.

### Flux de travail d'ingénierie de prompts
Notre [banc d'essai d'exemples de prompts Claude for Sheets](https://docs.google.com/spreadsheets/d/1sUrBWO0u1-ZuQ8m5gt3-1N5PLR6r%5F%5FUsRsB7WeySDQA/copy) est une feuille de calcul alimentée par Claude qui contient des exemples de prompts et des structures d'ingénierie de prompts.

### Modèle de classeur Claude for Sheets
Faites une copie de notre [modèle de classeur Claude for Sheets](https://docs.google.com/spreadsheets/d/1UwFS-ZQWvRqa6GkbL4sy0ITHK2AhXKe-jpMLzS0kTgk/copy) pour commencer votre propre travail avec Claude for Sheets !

## Dépannage et informations complémentaires
Pour plus d'informations concernant cette extension, consultez la page de présentation de [Claude for Sheets sur Google Workspace Marketplace](https://workspace.google.com/marketplace/app/claude%5Ffor%5Fsheets/909417792257).