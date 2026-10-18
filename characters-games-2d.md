# Personagens 2D — catálogo da casa

> Levantado em **18/10/2026** varrendo os repositórios de game (branch de trabalho de cada um).
> **Antes de gerar um personagem novo, procure aqui** (Ctrl+F pelo bicho, pela pose ou pela palavra-chave).
> Se existir, reaproveite: a arte-fonte (PNG / MP4) está no caminho indicado.

## Como ler

| Coluna | O que significa |
|---|---|
| **Personagem / arquivo** | nome do arquivo-fonte, sem extensão (o mesmo nome costuma existir como `.webp` no `APK/src/assets/sprites/`) |
| **Descrição** | o que é e qual papel tem no jogo |
| **Animação** | 🎬 **vídeo** = existe `.mp4` com fundo de chroma (verde ou magenta) e/ou folha `.webp` animada · 🖼️ **quadros** = poucos quadros soltos · ❌ **estático** = só a imagem |
| **Onde** | repositório e pasta |
| **Arte** | tipo de arte / estilo visual |

Legenda de estilos usados abaixo:

- **Cartoon IA BK** — ilustração cartoon colorida, contorno escuro, gerada por IA (`gpt-image-1`) a partir da referência oficial do Banana King. Mesmo estilo em Skyfall, Hook, Sky Pilot, Speed Boat, Wild West e Sky Adventure: **misturam-se entre si sem retoque**.
- **Pixel art** — sprite de baixa resolução, paleta limitada (Rampage, Defender).
- **Anime / K-pop semi-realista** — ilustração de personagem adulta estilo idol (kpop-dance, kpop-jump).
- **Cartoon K-pop** — cartoon mais simples e "fofo" (K-Pop Secret Agents). ⚠️ Nari/Yuna/Sora daqui **não** são as mesmas do kpop-dance/kpop-jump.

Convenções de nome dos arquivos que valem para quase todos os jogos BK:
`base-*` = imagem-base com fundo verde/magenta usada para gerar o vídeo · `bk-*` = Banana King · `ini-*` = inimigo · `chefe-*` = chefe · `*-derrotado` = pose de derrota · `*-folha` = folha de animação pronta.

---

## 1. Banana King (o herói da franquia)

O BK é o mesmo personagem em todos os jogos: **gorila jovem, camiseta amarela com uma banana no centro, coroa dourada** (variações por jogo abaixo). A referência mestre fica em cada projeto como `referencia/bk*.png` / `ref-bk-*` / `bk-referencia*`.

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `bk-referencia-paraquedista` / `bk-referencia-paraquedista-v1-com-paraquedas` | BK de frente, paraquedista (com e sem paraquedas) | ❌ | BANANA-KING-SKYFALL `PROJECT/assets/gerados/` | Cartoon IA BK |
| `base-bk-queda` (+ `-chroma`) → `bk-queda.mp4` | BK em queda livre, de barriga para baixo, olhando a câmera | 🎬 | SKYFALL `gerados/` e `videos/` | Cartoon IA BK |
| `bk-paraquedas.mp4`, `bk-pouso.mp4` (`bk-poso`, `bk-pouso-chroma`) | Abrindo paraquedas / pousando no alvo | 🎬 | SKYFALL `videos/` | Cartoon IA BK |
| `bk-lancar.mp4`, `bk-bonus-mirar.mp4`, `bk-bonus-lancar.mp4` (`base-bk-bonus-mirar`) | Lançando a banana bumerangue; mirar/lançar na fase bônus | 🎬 | SKYFALL `videos/` | Cartoon IA BK |
| `bk-dano.mp4`, `bk-derrota-queda.mp4` | Levando dano / caindo derrotado | 🎬 | SKYFALL `videos/` | Cartoon IA BK |
| `base-bk-congelado` → `bk-congelado.mp4` | BK congelado (cenário de gelo) | 🎬 | SKYFALL | Cartoon IA BK |
| `base-bk-enterrado` → `bk-enterrado.mp4` | BK enterrado no chão (pouso ruim) | 🎬 | SKYFALL | Cartoon IA BK |
| `base-bk-comemorando` → `bk-comemorando.mp4` | Comemorando | 🎬 | SKYFALL | Cartoon IA BK |
| `ui-bk-inicial`, `recorte-mockup-bk` | BK da tela inicial | ❌ | SKYFALL | Cartoon IA BK |
| `bk-parado`, `bk-balancando`, `bk-voando`, `bk-dano`, `bk-comemorando`, `bk-acenando`, `bk-acenando-2`, `bk-final` | 6 poses do BK de gancho/balanço + tela final | ❌ (poses soltas) | BANANA-KING-HOOK `PROJECT/assets/gerados/` | Cartoon IA BK |
| `idle.mp4` → `bk-idle.webp`, `caminhando.mp4` → `bk-andar.webp` | BK parado respirando / andando | 🎬 | HOOK `PROJECT/assets/` | Cartoon IA BK |
| `gorila-tela-inicial` | BK da tela inicial do Hook | ❌ | HOOK `PROJECT/assets/` | Cartoon IA BK |
| `ref-bk-piloto`, `ref-bk-sem-paraquedas`, `bk-em-pe` | BK piloto (sem paraquedas, cachecol vermelho) | ❌ | BANANA-KING-SKY-PILOT `PROJECT/assets/gerados/` | Cartoon IA BK |
| `base-bk-pilotando` (+`-16x9`) → `bk-pilotando.mp4` | BK pilotando o aviãozinho amarelo | 🎬 | SKY-PILOT `gerados/` e `videos/` | Cartoon IA BK |
| `bk-decolagem.mp4`, `bk-pouso-piloto.mp4`, `bk-atirando.mp4`, `bk-dano-piloto.mp4` | Decolagem, pouso, atirando míssil-banana, dano | 🎬 | SKY-PILOT `videos/` | Cartoon IA BK |
| `base-bk-ejetando` → `bk-ejetando.mp4` | BK ejetando do avião | 🎬 | SKY-PILOT | Cartoon IA BK |
| `base-bk-comemorando-piloto`, `base-bk-aviao-solo`, `bk-aviao-splash` | Comemorando de piloto; avião sozinho; arte de splash | ❌ / base | SKY-PILOT | Cartoon IA BK |
| `bk-referencia` (`referencia/bk-referencia.webp`) | Referência do BK de óculos de piloto laranja | ❌ | BANANA-KING-SPEED-BOART `PROJECT/assets/referencia/` | Cartoon IA BK |
| `base-bk-lancha-classica / -banana-jet / -coral / -onda-azul / -real / -trovao / -turbo` → `bk-lancha-*-folha` | BK pilotando cada uma das 7 lanchas | 🎬 (folha `-folha`) | SPEED-BOART `gerados/`, `bases-video/`, `videos/` | Cartoon IA BK |
| `base-bk-lancha-salto` → `bk-lancha-salto` | BK saltando a rampa com a lancha | 🎬 | SPEED-BOART | Cartoon IA BK |
| `base-bk-comemorando`, `bk-tela-inicial`, `ui-bk-inicial` | Comemorando; BK da tela inicial na lancha | 🎬 / ❌ | SPEED-BOART | Cartoon IA BK |
| `bk` (`referencia/bk.png`) | Referência do BK caubói | ❌ | BANANA-KING-Wild-West-Adventure `PROJECT/assets/referencia/` | Cartoon IA BK |
| `base-bk-cavalo-faisca / -cometa / -pintado / -real / -relampago / -trovao-negro` → `bk-cavalo-*` | BK montado em cada um dos 6 cavalos | 🎬 | WILD-WEST `gerados/`, `videos/` | Cartoon IA BK |
| `base-bk-arremesso`, `base-bk-chegada`, `base-bk-comemorando`, `base-bk-queda` → `bk-*` | Arremessando banana; chegada; comemorando; queda cômica | 🎬 | WILD-WEST | Cartoon IA BK |
| `ref-bk-parapente-voo`, `bk-franquia-skyfall` | BK de parapente; BK da franquia como referência | ❌ | banana-king-sky-adventure `PROJECT/assets/` | Cartoon IA BK |
| `base-bk-planando` → `bk-voo`, `base-bk-lancamento` → `bk-lancamento`, `base-bk-comemorando` → `bk-comemorando`, `bk-chegada` | Planando de parapente, saltando da rampa, comemorando, chegada | 🎬 | SKY-ADVENTURE `imagens/`, `APK/src/assets/sprites/` | Cartoon IA BK |
| `bk-inicial`, `bk-tela-inicial`, `ui-bk-cabeca` | BK da tela inicial; cabeça para HUD | ❌ | SKY-ADVENTURE | Cartoon IA BK |
| `personagem-bk-mov-v02` (v01 descartado) | BK visto de cima andando (top-down) | 🎬 vídeo + quadros | banana-king-rampage `PROJECT/assets/` | Pixel art (convertido de vídeo) |
| `Banana-king-frente-idle`, `banana-king`, `banana-king-costas`, `gorilla-f2` | BK de frente / de costas / quadro de andar | 🖼️ | RAMPAGE | Pixel art |
| `idle.mp4` → `ui-bk-aceno`, `banana-king-tela-inicial`, `ui-bk-inicial` | BK acenando (tela final e inicial, WebP animado) | 🎬 | RAMPAGE | Cartoon / pixel |
| `banana-king`, `banana-king-militar`, `banana-king-vitoria` | BK militar (defensor) e pose de vitória | ❌ | banana-king-defender `PROJECT/assets/` | Pixel art / cartoon |
| `banana-king-no-espaco` (+ `-espelhado`, `_branco`) | BK de traje espacial (herói do shooter) | ❌ | BANANA-KING-COUNTERATTACKS `PROJECT/assets/` | Cartoon |
| `win_Walk-Frame-1..5` (`-Phone`/`-Tablet`), `win_cheer` | BK andando/comemorando na tela de vitória | 🖼️ 5 quadros | COUNTERATTACKS `PROJECT/assets/`, `APK/public/assets/` | Cartoon |
| `gorila-frente-banana-01.svg` | BK vetorial de frente | ❌ | COUNTERATTACKS `APK/public/assets/` | Vetor |

---

## 2. Inimigos e vilões — família Banana King

### 2.1 Animais voadores (céu)

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `ini-aguia`, `ini-aguia-rasante`, `ini-aguia-derrotada`, `Águia Careca em Investida Dramática` | Águia inimiga (voando, rasante, derrotada) | 🖼️ poses | SKYFALL `gerados/`; também SKY-ADVENTURE `imagens/` | Cartoon IA BK |
| `ini-gaivota` (+`-derrotada`) → `ini-gaivota.mp4` | Gaivota | 🎬 | SKYFALL; SKY-ADVENTURE; SPEED-BOART (`base-ini-gaivota`, `ini-gaivota-folha`) | Cartoon IA BK |
| `ini-morcego` (+`-derrotado`) → `ini-morcego.mp4` | Morcego | 🎬 | SKYFALL; SKY-ADVENTURE | Cartoon IA BK |
| `ini-passaro` (+`-derrotado`), `hook-passaro-voando`, `passaro-voando`, `passaro-derrotado` | Pássaro vilão | 🖼️ | HOOK `gerados/`; SKYFALL; SKY-ADVENTURE | Cartoon IA BK |
| `bonus-passaro-bomba` (+`-chromakey`) → `bonus-passaro-bomba.mp4` | Pássaro-bomba (fase bônus) | 🎬 | SKYFALL; SPEED-BOART (`ini-passaro-bomba-folha`) | Cartoon IA BK |
| `bonus-passaro-dourado` → `bonus-passaro-dourado.mp4` | Pássaro dourado (bônus) | 🎬 | SKYFALL; SPEED-BOART | Cartoon IA BK |
| `ini-aviaozinho` (+`-derrotado`) | Aviãozinho inimigo | ❌ | SKYFALL | Cartoon IA BK |
| `ini-urubu` | Urubu | 🎬 | WILD-WEST | Cartoon IA BK |
| `papagaio-vilao-praia` | Papagaio vilão | 🎬 | RAMPAGE | Pixel art |
| `vilao-prehistoria-aerodactyl` (+`-chroma`) | Aerodáctilo | 🎬 | RAMPAGE | Pixel art |
| `inimigo-pombo` (+`-v02`, `pombo-frame-01..04`) | Pombo (cidade) | 🎬 | RAMPAGE | Pixel art |
| `abelha` (`-v02`, `-v03`) | Abelha | 🎬 | RAMPAGE | Pixel art |
| `inimigo-robo-voador` | Drone/robô voador | 🎬 | RAMPAGE | Pixel art |

### 2.2 Macacos / gorilas

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `gorila-parado`, `gorila-arremesso`, `gorila-derrotado` (e `hook-gorila-*` no Skyfall) | Gorila que joga cocos | 🖼️ 3 poses | HOOK `gerados/`; SKYFALL | Cartoon IA BK |
| `ini-macaco-bandana` (+`-arremesso`, `-derrotado`) → `.mp4` | Macaco de bandana | 🎬 | SKYFALL | Cartoon IA BK |
| `base-ini-macaco-pedra` / `ini-macaco-pedra` | Macaco que joga pedra | 🎬 | SPEED-BOART | Cartoon IA BK |
| `vilao-Trasho` (+`-espelhado`) | **Trasho**, chimpanzé vilão do shooter | ❌ | COUNTERATTACKS | Cartoon |

### 2.3 Terrestres e aquáticos

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `cobra-parada`, `cobra-derrotada` | Cobra | 🖼️ | HOOK `gerados/` | Cartoon IA BK |
| `inimigo-javali` | Javali | 🎬 | RAMPAGE | Pixel art |
| `inimigo-rato` (`-v02`, `-v03`) | Rato | 🎬 (5 quadros) | RAMPAGE | Pixel art |
| `vilao-inverno-lobo / -mamute / -pinguim / -urso` (+`-chroma`), `urso-vilao-fantasia` | Lobo, mamute, pinguim, urso polar | 🎬 | RAMPAGE | Pixel art |
| `vilao-prehistoria-tiranosauro` (+`-chroma`) | Tiranossauro | 🎬 | RAMPAGE | Pixel art |
| `inimigo-robo`, `inimigo-blindado` | Robô de fábrica; blindado | 🎬 / ❌ | RAMPAGE | Pixel art |
| `base-ini-boto, -caranguejo, -carpa, -hipopotamo, -jacare, -peixe-fogo, -pinguim, -polvo, -tubarao` → `ini-*` (+ `ini-baiacu`, `ini-peixe`) | Fauna aquática inimiga (12 cenários) | 🎬 (folhas) | SPEED-BOART `gerados/`, `bases-video/` | Cartoon IA BK |
| `base-ini-gondoleiro, -pirata-esqueleto, -viking, -rival` → `ini-*` | Gondoleiro, pirata esqueleto, viking, lancha rival (BK adversário) | 🎬 | SPEED-BOART | Cartoon IA BK |
| `base-ini-rebocador`, `ini-barquinho`, `ini-veleiro`, `ini-cargueiro` | Barcos inimigos (objeto-personagem) | 🎬 / ❌ | SPEED-BOART | Cartoon IA BK |
| `base-ini-bandido`, `base-ini-bandido-cavalo` → `ini-*` | Bandido a pé / a cavalo | 🎬 | WILD-WEST | Cartoon IA BK |
| `base-ini-cacto-vivo`, `base-ini-cacto-gigante` | Cacto vivo / gigante (recorte magenta) | 🎬 | WILD-WEST | Cartoon IA BK |
| `base-ini-coiote, -escorpiao, -touro, -cabra` | Coiote, escorpião, touro, cabra | 🎬 | WILD-WEST | Cartoon IA BK |
| `base-ini-fantasma`, `base-ini-minerador` | Fantasma; minerador | 🎬 | WILD-WEST | Cartoon IA BK |
| `base-ini-robo-pistoleiro, -automato, -vaca-robo, -drone, -guarda-alien, -canhao-neve, -draisine` | Robôs e alienígenas do Oeste futurista | 🎬 | WILD-WEST | Cartoon IA BK |
| `inimigo-soldado-raso`, `inimigo-tanque` | Soldado raso e tanque (tower defense) | 🖼️ (andar derivado) | banana-king-defender `PROJECT/assets/sprites/` | Pixel art militar |
| `nave-inimiga-00..05` | Naves da tropa do Trasho | ❌ | COUNTERATTACKS `APK/public/assets/` | Cartoon |

### 2.4 Chefes

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `base-chefe-capitao-macaco` → `chefe-capitao-macaco.mp4` | Capitão macaco | 🎬 | SKYFALL | Cartoon IA BK |
| `base-chefe-dragao-pipa` → `chefe-dragao-pipa.mp4` | Dragão-pipa | 🎬 | SKYFALL; SPEED-BOART (`ini-dragao-pipa-folha`) | Cartoon IA BK |
| `base-chefe-gorila-gelo` → `chefe-gorila-gelo.mp4` | Gorila de gelo | 🎬 | SKYFALL | Cartoon IA BK |
| `base-chefe-rei-sombrio` → `chefe-rei-sombrio.mp4` | Rei sombrio (vilão final) | 🎬 | SKYFALL | Cartoon IA BK |
| `base-chefe-boiuna, -cargueiro, -doge-macaco, -dragao-agua, -esfinge-flutuante, -golem-magma, -jacarezao, -kraken, -morsa-gigante, -navio-sombrio, -rei-caranguejo, -rei-viking` → `chefe-*-folha` | 12 chefes, um por cenário | 🎬 (folhas) | SPEED-BOART | Cartoon IA BK |
| `zorg` / `base-zorg` (`referencia/zorg.png`) | **Zorg**, vilão alienígena | 🎬 | WILD-WEST | Cartoon IA BK |
| `nave`, `nave-final` (`base-nave*`) | Nave do Zorg (foge / batalha final) | 🎬 | WILD-WEST | Cartoon IA BK |

### 2.5 Aliados, NPCs e montarias

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `mimosa` / `base-mimosa` | **Mimosa**, a vaquinha do BK (abduzida) | 🎬 | WILD-WEST | Cartoon IA BK |
| `npc-*` (12: dusty-ranch, ghost-town, gold-rush, red-canyon, storm-valley, neon-frontier, iron-horse, bone-valley, steamworks, frozen-frontier, alien-outpost, stronghold) | Um NPC de chegada por cidade | 🎬 | WILD-WEST | Cartoon IA BK |
| `loja-cavalo-*` (6) | Cavalos da loja (Faísca, Cometa, Pintado, Real, Relâmpago, Trovão Negro) sem o BK | ❌ | WILD-WEST | Cartoon IA BK |
| `loja-lancha-*` (6) | Lanchas da loja sem o BK | ❌ | SPEED-BOART | Cartoon IA BK |
| `aviao-bimotor` (+`-chromakey`) → `aviao-bimotor.mp4` | Bimotor de onde o BK salta | 🎬 | SKYFALL | Cartoon IA BK |
| `ref-aviao-jogador`, `obs-aviao-carreira`, `ini-aviao-cauda` | Aviãozinho amarelo do BK; avião de carreira | ❌ | SKY-PILOT | Cartoon IA BK |

---

## 3. K-pop — dançarinas e agentes

### 3.1 K-Pop Dance (6 dançarinas adultas, 19–21 anos)

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `YUNA`, `YUNA-pose02`, `YUNA-assets`, `CHROMA-YUNA`, `yuna-retrato` | Yuna (dançarina inicial, livre) | 🎬 vídeo chroma → dança VP9 | kpop-dance `PROJECT/fontes-assets/`, `APK/src/assets/imagens/` | Anime / K-pop semi-realista |
| `SORA` (…) | Sora (exceção de figurino: barriga) | 🎬 | kpop-dance | idem |
| `MINA` (…) | Mina | 🎬 | kpop-dance | idem |
| `HANA` (…) | Hana | 🎬 | kpop-dance | idem |
| `RINA` (…) | Rina (dança provisória em loop de 2 s) | 🎬 | kpop-dance | idem |
| `NARI`, `chroma-NARI` (…) | Nari (turquesa puxado ao ciano) | 🎬 | kpop-dance | idem |

### 3.2 KPOP Jump (4 avatares de pular corda)

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `AVATAR-01` / `nari-*` | **NARI** — cabelo ombré, jeans rasgado | 🎬 clipes `danca`, `pulo`, `queda` (6 quadros WebP cada) | kpop-jump `PROJECT/assets/`, `avatares/`, `frames-png/` | Anime / K-pop semi-realista |
| `AVATAR-02` / `rinae-*` | **RINAE** — ídolo estelar azul e preto | 🎬 idem | kpop-jump | idem |
| `AVATAR-03` / `aerin-*` | **AERIN** — ídolo neon punk (jaqueta com estrela) | 🎬 idem | kpop-jump | idem |
| `AVATAR-04` / `veli-*` | **VELI** — garota cyber-gótica roxo e prata | 🎬 idem | kpop-jump | idem |

### 3.3 K-Pop Secret Agents (3 espiãs, cartoon)

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `Nari`, `base-nari-perfil`, `nari-parada/-idle/-correndo/-pulo/-lancando/-dano` | **Nari** (amarelo, estrelas, pulo duplo) | 🎬 (6 ações) | K-Pop-Secret-Agents `PROJECT/assets/`, `gerados/`, `videos/` | Cartoon K-pop (chroma magenta) |
| `YUNA`, `base-yuna-perfil`, `yuna-*` | **Yuna** (vermelho, corações, arrancada) | 🎬 | idem | idem |
| `Sora`, `base-sora-perfil`, `sora-*` | **Sora** (verde, cristais, leque de 3) | 🎬 | idem | idem |
| `inimigo-abelha`, `inimigo-pombo`, `inimigo-rato`, `inimigo-robo` (+`-anim`) | Inimigos comuns | 🎬 | idem | idem |
| `inimigo-b01-esquilo`, `-b02-ganso`, `-b03-macaco` / `chefe-b01..b03` | Inimigo exclusivo e mini-chefe dos blocos 1–3 | 🎬 (b01) / ❌ | idem | idem |
| `missao-b01-gato-java` | Gato Java a resgatar (missão bloco 1) | ❌ | idem | idem |

---

## 4. Outros jogos

| Personagem / arquivo | Descrição | Animação | Onde | Arte |
|---|---|---|---|---|
| `mascote` | Mascote cogumelo de MushRush (tela inicial) | ❌ | MushRush `PROJECT/assets/` | Cartoon brilhante |
| `cogumelos.png`, `fungos-dourados.png` (recortes em `sprites/`) | 24 cogumelos (12 lisos + 12 ornados) — peças do jogo | ❌ | MushRush `PROJECT/assets/`, `sprites/` | Cartoon |
| `gato`, `Perseguição Felina em Pleno Salto` | Arte 2D do gato Java (conceito/tela) | ❌ | Mouse-Hunt `PROJECT/FONTS-ASSETS/` | Cartoon 3D-render (conceito) |
| `mouse`, `mouse_v2` | Arte 2D do rato | ❌ | Mouse-Hunt `PROJECT/FONTS-ASSETS/` | idem |

---

## Projetos sem personagem 2D

- **kako-steel** — os personagens são 3D (ver `characters-games-3d.md`).

## Observações para o ilustrador

- Os vídeos `.mp4` têm fundo de **chroma verde** (ou **magenta** onde o personagem é verde: cactos do Wild West, todo o K-Pop Secret Agents). Recortar com o `tools/preparar-animacoes.mjs` do projeto (excesso de cor), **não** com o `chromakey` do ffmpeg.
- Uma `base-*.png` existente pode gerar **novas animações** do mesmo personagem sem nova imagem.
- ⚠️ Nari/Yuna/Sora existem em **três** projetos e são **personagens diferentes** — conferir o projeto antes de reaproveitar.
