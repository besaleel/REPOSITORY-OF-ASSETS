# Personagens 3D — catálogo da casa

> Levantado em **18/10/2026** varrendo os repositórios de game. **Antes de modelar um personagem 3D novo, procure aqui.**
> Hoje só **dois** projetos têm personagens 3D: **Mouse-Hunt** (Unity) e **kako-steel** (Three.js).

## Como ler

| Coluna | O que significa |
|---|---|
| **Personagem / arquivo** | nome do modelo |
| **Descrição** | o que é e o papel no jogo |
| **Rig** | ✅ esqueleto (ossos) · ❌ malha estática · ❓ não conferido |
| **Animação** | clipes existentes |
| **Onde** | repositório e caminho |
| **Arte** | tipo de arte / estilo e orçamento |

---

## Mouse-Hunt — *Java the Mouse Hunter* (Unity 6)

| Personagem / arquivo | Descrição | Rig | Animação | Onde | Arte |
|---|---|---|---|---|---|
| `CHR_Cat` (`.fbx`, `.glb`, `.blend`) | **Java**, o gato caçador (personagem jogável) | ✅ 48 ossos | ✅ `CHR_CatAnims.fbx` / `CHR_Cat_anim.blend`: `Cat_Idle`, `Cat_Walk`, `Cat_Run`, `Cat_Pounce` (procedurais, script `cat_animations.py`). Animator Generic, sem Avatar | `APK/Assets/Art/Characters/`; fontes em `PROJECT/3D-assets-otimizados-v2/{fbx,glb,blend}/`; original em `PROJECT/3d-personagens/cat.glb` | 3D cartoon estilizado, gerado por IA (Tripo AI) e otimizado no Blender |
| `CHR_Mouse` (`.fbx`, `.glb`, `.blend`) | O rato fugitivo (IA/NPC) — nunca é ferido | ❓ a conferir (anotado na `RETOMADA.md`) | ❌ sem clipes | idem; original `PROJECT/3d-personagens/mouse.glb` | idem |
| `CHR_Mouse_v1_bocaaberta` | Variante do rato de boca aberta (susto/pânico) | ❓ | ❌ | `PROJECT/3D-assets-otimizados-v2/`; original `mouse_v1_bocaaberta.glb` | idem |

> ⚠️ Os `.glb`/`.fbx` deste projeto estão em **Git LFS**: é preciso `git lfs pull` para baixar o modelo real.
> Arte 2D de referência dos dois personagens: `PROJECT/FONTS-ASSETS/gato.png`, `mouse.png`, `mouse_v2.png`.

## kako-steel — simulação de siderúrgica (Three.js, `.glb` riggados)

> ⚠️ A pasta-fonte `PROJECT/assets/` **não é versionada**: os `.glb` estão na máquina do dono. As especificações vêm de `DOCUMENTAÇÃO/ASSETS.md` §2.

| Personagem / arquivo | Descrição | Rig | Animação | Onde | Arte |
|---|---|---|---|---|---|
| `kako.glb` (fonte `kako_Merged_Animations.glb`) | **Kako**, mascote-guia | ✅ 24 ossos | ✅ 8 clips no bundle (`idle`, `point`, `worried`, `victory`, `walk`… ) + 3 só no fonte (`Wave_One_Hand`, dois sentados) | `assets/3d/kako.glb`; fonte `PROJECT/assets/glb/` | 3D toon, 5.079 tris, textura 1024² WebP, 818 KB |
| `worker.glb` (fonte `worker_Merged_Animations.glb`) | Operador de produção, instanciado até 24× | ✅ | ✅ 5 clips no bundle (12 no fonte, ex.: `open_door_3`) | `assets/3d/worker.glb` | 3D toon, 2.463 tris, 512², capacete trocável (amarelo/azul/verde) |
| `forklift.glb` | Empilhadeira (veículo-ator) | ✅ 6 ossos | ✅ `idle`, `drive`, `lift` | `assets/3d/` | Low-poly modelado à mão (script), 456 tris |
| `truck_hopper.glb` | Carreta de minério | ✅ | ✅ `drive`, `dump` | `assets/3d/` | Low-poly, 438 tris |
| `truck_flatbed.glb` | Caminhão de placa/bobina | ✅ | ✅ `drive`, `load` | `assets/3d/` | Low-poly, 522 tris |
| `torpedo.glb` | Carro torpedo (gusa) | ✅ | ✅ `move` + emissivo pulsante | `assets/3d/` | Low-poly, 568 tris |

---

## Jogos sem personagem 3D

Todos os jogos Banana King, K-pop e MushRush são **2D** — ver `characters-games-2d.md`.
(O `Meshy_AI_Gameplay Prototype Banana Barriers.png` do COUNTERATTACKS é só imagem de conceito, não modelo.)
