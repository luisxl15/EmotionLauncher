# EmotionLauncher
A launcher for PCSX2 for a look more like a console

<div align="center">

# 🎮 Emotion Launcher

**Um front-end no estilo PlayStation para o emulador PCSX2.**

Organize, decore e jogue sua biblioteca de PlayStation 2 numa interface XMB com fundo de ondas animado, fonte *EmotionEngine*, conquistas, arte de capa automática e navegação total por controle.

</div>

---

## ✨ O que é

O **Emotion Launcher** transforma sua coleção de jogos de PS2 numa experiência de console: você abre o programa, navega pelos jogos com o controle (ou mouse/teclado), vê capas, descrições, progresso de conquistas e tempo jogado — e dá *play*. Ele cuida de abrir o PCSX2 com as configurações certas pra cada jogo.

Tudo roda offline; os recursos online (capas, descrições, conquistas) são **opcionais** e só ligam se você quiser.

---

## 🌟 Funcionalidades

### 🖥️ Interface
- **Dashboard XMB** estilo PS4/PS5, com fundo de ondas em *canvas* e a fonte oficial *EmotionEngine*.
- Mostra os **3 últimos jogos jogados** em destaque + atalhos (Biblioteca, Progresso, Coleções, Estatísticas, Mídia, Memory Cards, Configurações).
- **Música de fundo** em loop e **sons de navegação** (com liga/desliga).
- **Animação de boot** estilo PS2 ao abrir.
- **3 idiomas**: Português, Inglês e Espanhol.
- Temas de cor (azul / prata / branco).

### 📚 Biblioteca
- **Escaneia todos os formatos** de PS2: `.iso` `.bin` `.img` `.mdf` `.nrg` `.cso` `.zso` `.gz` `.chd` `.cue` `.mds` `.dump`.
- Lê o **serial** direto do disco (ou do nome do arquivo) e resolve o **título oficial**.
- Visualizações em grade, lista e carrossel; busca e filtros.
- **Coleções personalizadas** — agrupe jogos em listas próprias (ex.: "Zerar", "Co-op", "Clássicos").
- **Suporte multi-disco** — vincule disco 2/3 e escolha qual rodar ao iniciar.
- **Continue Playing** — retome do save state mais recente.

### 🖼️ Tela de detalhe enriquecida
- Capa, fundo *widescreen*, descrição, gênero, ano, desenvolvedora, publicadora, região e jogadores.
- **Barra de progresso de conquistas** + emblemas (desbloqueados em destaque).
- **Galeria de screenshots** do jogo (puxadas da pasta do PCSX2).
- Tempo jogado, número de partidas e **selo de compatibilidade** colorido.

### 🏆 Conquistas
- **Por jogo**: lista completa com pontos e quais você desbloqueou.
- **Aba Progresso**: visão geral do seu RetroAchievements — conquistas ganhas, jogos completados, pontos e rank.

### 🎮 Controle
- **Navegação 100% por gamepad** — funciona em todas as telas **e também nos menus** (menu de contexto, seletores, configurações).
- **Remapeamento de botões** (Confirmar / Voltar / Opções).
- Símbolos dos botões do PS2 (○ × □ △) desenhados nas **cores originais da Sony**.
- **Start + Select fecha o jogo** e volta pro launcher.
- **Scroll do mouse** navega pelos lados no dashboard.

### ⚙️ Emulação
- **Configurações por jogo** (renderizador, resolução, *aspect ratio*, *speedhacks*, patches, tela cheia) gravadas direto no `PCSX2.ini`.
- **Compatibilidade automática** de cada jogo (offline).
- Inicia o jogo já com tudo aplicado; **boot direto na BIOS** do PS2 também disponível.
- **Cheats** (`.pnach`): liste e ative/desative por jogo.
- **Gerenciador de Memory Cards**: criar, apagar e fazer backup.
- Chip **"Jogando agora"** + **contagem real de tempo** (monitora o processo do PCSX2).

### 🔧 Extras
- **Setup inicial** que pode **baixar e instalar o PCSX2** pra você (último release oficial).
- **Verificador de atualizações** do próprio launcher.
- **Discord Rich Presence** — mostra o que você está jogando.
- Dados salvos em **`Documentos\Emotion Launcher`** (fácil de achar e fazer backup).

---

## 🔌 Integrações & APIs

O launcher conversa com alguns serviços pra enriquecer a experiência. Cada um é **opcional** e tem uma função específica:

| Serviço | Pra que serve | Precisa de chave? | Onde conseguir |
|---|---|---|---|
| **TheGamesDB** | **Descrição** dos jogos (sinopse, gênero, ano, etc.) | ✅ API key gratuita | [thegamesdb.net](https://thegamesdb.net) |
| **Wikipedia** | **Descrição** alternativa (usada se não tiver TheGamesDB) ✅
| **SteamGridDB** | **Capas** (grids) e **fundos/banners** (heroes) — automático ou seletor manual | ✅ API key gratuita | [steamgriddb.com](https://www.steamgriddb.com) |
| **RetroAchievements** | **Conquistas** por jogo e a **aba Progresso** | ✅ usuário + Web API key | [retroachievements.org/settings](https://retroachievements.org/settings) |
| **PCSX2 GameIndex.yaml** | **Títulos oficiais** + **compatibilidade** dos jogos ✅
| **Discord** | **Rich Presence** (mostra o jogo no seu perfil) ✅
| **GitHub Releases** | **Baixar/instalar o PCSX2** e **checar updates** do launcher ✅

> As chaves de API são coladas em **Configurações** (TheGamesDB e RetroAchievements em suas respectivas seções; SteamGridDB em *Artwork*). Sem elas, o launcher funciona normalmente — só não busca capa/descrição/conquistas online.

### ⚠️ Sobre as conquistas
O launcher **mostra** seu progresso do RetroAchievements via API. Para **ganhar** conquistas, você precisa ativar a opção *Achievements* **dentro do próprio PCSX2** e logar com sua conta RA lá — é o emulador que registra os desbloqueios.

---

## 📦 Requisitos

- **Windows 10/11** (64-bit).
- **PCSX2** (versão Qt) — você pode **baixar pelo próprio setup** do launcher, ou apontar pra uma instalação existente.
- **BIOS do PlayStation 2** — extraída do **seu próprio console** (não é incluída).
- **Seus jogos** de PS2 (não são incluídos).
- *(Opcional)* chaves de API para capas, descrições e conquistas.
- *(Opcional)* um controle (Xbox / PlayStation / genérico XInput).

---

## 🚀 Instalação

1. Baixe o **`EmotionLauncherSetup.exe`** na aba [Releases](../../releases).
2. Rode o instalador, escolha a pasta e os atalhos, e clique em **Instalar**.
3. Abra o **Emotion Launcher**.

Na **primeira vez**:
1. Vá em **Configurações → Emulador** e aponte o **executável do PCSX2** (`pcsx2-qt.exe`) e a pasta da **BIOS** — ou use o setup pra baixar o PCSX2.
2. Em **Configurações → Biblioteca**, adicione as pastas dos seus jogos e clique em **Escanear**.
3. *(Opcional)* cole suas chaves de API pra buscar capas, descrições e conquistas. Capas são pelo SteamGrid DB, descrições são pelo The Games DB.

---

## 🎛️ Controles

| Entrada | Ação |
|---|---|
| Direcional / Analógico · Setas | Navegar |
| ○ Círculo · Enter | Confirmar / Jogar |
| × Cross · Esc | Voltar / Fechar menu |
| △ Triângulo · Start | Abrir menu de opções do jogo |
| **Start + Select** (em jogo) | Fechar o jogo e voltar ao launcher |
| Scroll do mouse | Navegar pelos lados (dashboard) |

---

## 📁 Onde ficam os dados

Configurações, biblioteca, capas e caches ficam em:

```
Documentos\Emotion Launcher\
```

É só apagar essa pasta para "zerar" o launcher.

---

## ⚖️ Aviso legal

O Emotion Launcher é apenas um **front-end** para o PCSX2. **Não distribui** a BIOS do PlayStation 2 nem jogos — você deve usar dumps da **sua própria** BIOS e dos **seus próprios** discos. *PlayStation*, *PS2* e *Emotion Engine* são marcas da Sony Interactive Entertainment; este projeto não é afiliado à Sony nem à equipe do PCSX2.
