# FocusLauncher

Launcher Android minimalista, rapido e personalizavel, pensado para manter no ecra principal apenas o que interessa.

Versao atual: `1.25` (`versionCode 25`)

## Autor

**Goncalo Garrido**  
Email: `goncalosantosgarrido@gmail.com`

## Visao Geral

O `FocusLauncher` e um launcher Android desenvolvido em Kotlin, com foco em:

- simplicidade visual
- acesso rapido a informacao util
- configuracao por ecra
- persistencia local
- experiencia fluida e minimalista

Em vez de um launcher pesado e cheio de elementos, o projeto organiza a experiencia em varios ecras deslizaveis, onde cada pagina pode ser ativada, ocultada, reordenada e configurada individualmente.

## O Que a App Faz

O launcher ja inclui:

- ecra principal com hora, data, bateria, progresso do dia e apps fixadas
- 9 layouts diferentes para o bloco de informacao da home
- editor de apps do ecra principal
- lista completa de apps com pesquisa, secoes alfabeticas e indice lateral
- ajuda para definir o launcher como predefinido
- tarefas com persistencia local
- agenda com proximos eventos do calendario
- meteorologia com estado atual e previsao de varios dias
- calculadora com historico
- notas com gravacao automatica local
- contactos favoritos em lista ou grelha
- historico de notificacoes por categoria
- links guardados em grelha
- quick tools
- clipboard
- resumo do dia
- habit tracker
- temporizador de foco
- sudoku
- wordle / termo
- musica
- ChatGPT
- estado do sistema

## Ecras Disponiveis

As paginas atualmente suportadas incluem:

- Home
- Day Summary
- Weather
- Tasks
- Favorite Contacts
- Notification History
- Focus Timer
- Habit Tracker
- Widgets
- Quick Tools
- Clipboard
- App Drawer
- Links Grid
- Agenda
- Calculator
- Sudoku
- Wordle / Termo
- Music
- ChatGPT
- Notes
- System Status
- Customization

## Configuracao

O launcher permite configurar:

- ecras ativos
- ordem dos ecras ativos
- definicoes avancadas por ecra
- cor de fundo
- wallpaper do sistema como fundo
- cor do texto
- formato da hora
- formato da data
- visibilidade da hora
- visibilidade do progresso do dia
- estilo do progresso do dia
- estilo do indicador de bateria
- unidades de temperatura e vento
- idioma da app
- layout, densidade e apresentacao das apps da home

## Stack Tecnologica

- Kotlin
- Android SDK
- AndroidX
- Material Components
- ViewBinding
- SharedPreferences
- armazenamento interno
- SQLite
- Retrofit
- Gson Converter
- Google Play Services Location
- Picasso
- Kotlin Coroutines

## Estrutura do Projeto

```text
FocusLauncherApp/
|-- FocusLauncher.Android/
|   |-- app/
|   |   |-- src/main/java/com/example/launcher/
|   |   |-- src/main/res/
|   |-- build.gradle
|-- Res/
|   |-- PlayStore/
|-- README.md
```

## Componentes Principais

- `MainActivity`: contentor principal do launcher e gestor das paginas
- `HomeFragment`: home com informacao principal e apps fixadas
- `AppDrawerFragment`: lista completa de apps com pesquisa e navegacao alfabetica
- `LauncherSettingsActivity`: hub principal de configuracoes
- `ScreensSettingsActivity`: gestao dos ecras ativos e ordem
- `HomeContentSettingsActivity`: configuracao do conteudo e layouts da home
- `HomeAppsEditorFragment`: editor das apps fixadas

## Permissoes Utilizadas

- `QUERY_ALL_PACKAGES`
- `INTERNET`
- `ACCESS_NETWORK_STATE`
- `ACCESS_FINE_LOCATION`
- `ACCESS_COARSE_LOCATION`
- `READ_CALENDAR`
- `WRITE_CALENDAR`
- `READ_CONTACTS`
- `READ_EXTERNAL_STORAGE`
- `REQUEST_DELETE_PACKAGES`
- `CAMERA`
- `POST_NOTIFICATIONS`
- `com.android.alarm.permission.SET_ALARM`

## Executar

### Android Studio

1. Abrir a pasta `FocusLauncher.Android`
2. Esperar pela sincronizacao do Gradle
3. Selecionar um dispositivo ou emulador
4. Executar a app

### Linha de Comando

```powershell
cd FocusLauncher.Android
.\gradlew.bat assembleDebug
```

## Estado Atual

O projeto esta funcional e em evolucao ativa. O foco atual esta em:

- melhorar estabilidade
- alinhar a app com os requisitos atuais da Google Play
- polir a experiencia visual
- aumentar a flexibilidade das configuracoes
- continuar a expandir os ecras sem perder a identidade minimalista

## Licenca

Este repositorio nao tem licenca definida neste momento.
