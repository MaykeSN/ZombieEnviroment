# Meu Primeiro Ambiente VR — Apocalipse (Meta Quest)

Projeto em Unity com temática de **apocalipse** (ambiente destruído/abandonado), criado para demonstrar fundamentos básicos de XR/VR:
- cena navegável
- ambiente 3D com chão, skybox e objetos
- organização do projeto
- build preparado para **Android (Meta Quest)**
- testes iniciais no **PC (Unity Editor)**

---

## Tecnologias / Pacotes

- **Unity:** 6.3 LTS
- **Meta XR (All-in-One SDK / Building Blocks)**
- **OpenXR (XR Plug-in Management)**
  - **Meta Quest Support** habilitado (OpenXR Feature Group)

---

## Assets utilizados

- **Apocalypse: Playground Environment** (ambiente/cenário e props)

> Obs.: cheguei a testar um pack de zumbis, mas removi do projeto por problemas/bugs no meu cenário.

---

## Requisitos atendidos (checklist)

### 1) Configuração Técnica
- [x] Projeto Unity compatível com Meta XR
- [x] Meta XR SDK instalado e configurado (Building Blocks)
- [x] XR Plugin Management configurado com OpenXR + Meta Quest Support
- [x] Build Settings preparado para Android (Meta Quest)
- [x] Movimentação/testes no PC (Play Mode no Editor) sem depender do óculos

### 2) Ambiente Virtual
- [x] Pelo menos 5 objetos 3D na cena (assets importados e props)
- [x] Chão/terreno com colisão para caminhar
- [x] Skybox configurado
- [x] Objetos posicionados de forma coerente, criando um ambiente reconhecível

### 3) Organização e Qualidade
- [x] Hierarquia organizada por grupos (XR / iluminação / ambiente / props)
- [x] Nomenclatura consistente
- [x] Projeto limpo no Git (sem Library/Temp/etc.)
- [x] Documentação (este README)

---

## Como abrir o projeto

1. Abra a Unity Hub
2. **Open > Add project from disk**
3. Selecione a pasta do projeto
4. Abra a cena principal:
   - `Assets/_Project/Scenes/Main.unity` (ou a cena principal do projeto)

---

## Como testar no PC (sem Meta Quest)

1. Abra a cena principal
2. Garanta que o modo de testes no Editor está configurado
3. Clique **Play**
4. Navegue pela cena usando o setup de simulação do projeto

> Importante: mantenha **apenas 1 câmera/rig ativo por vez** para evitar conflitos.

---

## Como buildar para Meta Quest (Android)

1. **File > Build Settings…**
2. Selecione **Android** e clique **Switch Platform**
3. Em **Scenes In Build**, clique **Add Open Scenes**
4. **Edit > Project Settings… > XR Plug-in Management**
   - Aba **Android**: **OpenXR** habilitado
   - Em **OpenXR**: **Meta Quest Support** habilitado (Feature Group)
5. Clique **Build** (APK) ou **Build And Run**

---

## Organização (estrutura sugerida)

- `Assets/_Project/Scenes` — cenas do projeto
- `Assets/_Project/Art/Models` — modelos
- `Assets/_Project/Art/Materials` — materiais
- `Assets/_Project/Art/Textures` — texturas
- `Assets/_Project/Prefabs` — prefabs prontos (props, peças do cenário)
- `Assets/_Project/Scripts` — scripts
- `Assets/_Project/Docs` — docs extras (se necessário)

---

## Principais dificuldades (e como resolvi)

### 1) Configurar um ambiente “bom” (chão, skybox e iluminação)
A maior dificuldade foi montar um cenário coerente com chão funcional (colisão) e um visual agradável.
- Solução: usei o pack **Apocalypse: Playground Environment**, ajustei o chão/colisões e configurei skybox/iluminação para dar clima de apocalipse.

### 2) Rodar o simulador no PC (muito travado no início)
Tive dificuldade com a parte de simulação/teste no Editor: ficou travando e foi confuso entender o que precisava estar ligado/desligado.
- Solução: padronizei o uso de um único rig/câmera por vez, removi/disablei câmeras extras de packs e mantive a cena organizada para reduzir conflito e carga.

---

## Autor
- Mayke"# ZombieEnviroment" 
