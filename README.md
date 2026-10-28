<h1 align="center">VOID ADB</h1>
<p align="center"><b>Otimizador de jogos para Android, sem root.</b><br>
Trabalha pelo ADB, via Shizuku ou AxManager. Deixa a partida mais lisa, segura o calor, corta o que pesa em segundo plano e devolve tudo ao normal quando você desliga.</p>

<p align="center">
<a href="https://github.com/Ryuta290/VOID_ADB/raw/main/apk/VOID-ADB-v15.39.1.apk"><b>⬇️ Baixar VOID 15.39.1 (APK)</b></a> ·
<a href="https://github.com/Ryuta290/VOID_ADB/releases">Todas as versões</a>
</p>

---

## Sumário

1. [O que é o VOID](#o-que-é-o-void)
2. [Requisitos](#requisitos)
3. [Instalação passo a passo](#instalação-passo-a-passo)
4. [Primeiros passos](#primeiros-passos)
5. [As abas do app](#as-abas-do-app)
6. [Funções em detalhe](#funções-em-detalhe)
7. [Ferramentas](#ferramentas)
8. [Permissões e por que cada uma é usada](#permissões-e-por-que-cada-uma-é-usada)
9. [Segurança: as regras do VOID](#segurança-as-regras-do-void)
10. [Como desfazer tudo](#como-desfazer-tudo)
11. [Problemas comuns](#problemas-comuns)
12. [Perguntas frequentes](#perguntas-frequentes)
13. [Limitações conhecidas](#limitações-conhecidas)
14. [Novidades](#novidades)
15. [Verificar se o APK é oficial](#verificar-se-o-apk-é-oficial)
16. [Direitos](#direitos)

---

## O que é o VOID

O VOID ADB muda configurações do Android com o mesmo nível de acesso do ADB, o que um app comum não pode fazer. Com isso ele ajusta taxa de atualização da tela, memória, processos em segundo plano, rede e calor **na hora em que o jogo abre**, e desfaz tudo quando a partida acaba.

- **Sem root.** Usa Shizuku ou AxManager.
- **Mais de 160 funções e 22 ferramentas**, em quatro áreas: Jogo, Sistema, Rede e Ferramentas.
- **Tudo é reversível.** O valor original é salvo antes de cada mudança.
- **O botão ATIVAR manda.** Com o VOID desligado, nenhuma função age.
- Cada função tem um **"Saiba mais"**: o que muda, o que você vai notar, quando age, cuidados e como desfazer.
- Disponível em **português, inglês, espanhol e indonésio**.

## Requisitos

| Item | Detalhe |
|---|---|
| Android | 8.0 ou mais novo |
| Acesso | [Shizuku](https://shizuku.rikka.app/) **ou** AxManager ativo (Brevent como reserva) |
| Root | Não precisa |
| Espaço | cerca de 7 MB |

Funciona em qualquer marca. Em Samsung, Xiaomi/POCO/Redmi, OPPO/realme/OnePlus e outras, o VOID reconhece as chaves da própria marca e só usa as que já existem no aparelho.

## Instalação passo a passo

### 1. Instale o Shizuku
1. Baixe o Shizuku na Play Store ou no site oficial.
2. Ative as **Opções do desenvolvedor**: Configurações → Sobre o telefone → toque 7 vezes em "Número da versão".
3. Ative a **Depuração por Wi-Fi** (Android 11+) nas Opções do desenvolvedor.
4. Abra o Shizuku e toque em **Iniciar via depuração sem fio**. Siga o pareamento pela notificação.
5. Pronto quando o Shizuku mostrar "Shizuku está em execução".

> No Android 10 ou mais antigo, o Shizuku precisa ser iniciado uma vez pelo computador com `adb`. O próprio app explica o comando.
> Depois de reiniciar o celular, o Shizuku precisa ser iniciado de novo (sem root).

### 2. Instale o VOID
1. Baixe o APK pelo link no topo desta página.
2. Abra o arquivo e permita "instalar apps desconhecidos" para o navegador ou gerenciador de arquivos, se o Android pedir.
3. Se o Play Protect avisar, toque em **Mais detalhes → Instalar mesmo assim**. O aviso aparece com qualquer app fora da Play Store.

### 3. Primeira abertura
1. Depois da animação de entrada, o VOID pede a permissão do Shizuku. Toque em **Permitir sempre**.
2. Ele pede notificações (pro serviço da partida) e, quando você usar, Acessibilidade e Sobreposição.
3. Na aba **Início**, o status mostra o que está ligado e funcionando.

### Atualizar
Instale o APK novo por cima. As configurações ficam.

## Primeiros passos

1. Vá na aba **Jogo** e adicione seus jogos à lista.
2. Escolha um **Perfil pronto** na aba Início (por exemplo, Equilibrado ou Competitivo).
3. Toque em **ATIVAR**.
4. Abra o jogo. O VOID prepara o celular sozinho e mostra o **Balão VOID** com FPS e temperatura.
5. Saia do jogo: tudo volta ao normal.

Dica: comece com poucas funções, jogue uma partida e use o **Antes e Depois** e a **Prova por função** pra ver o que realmente fez diferença no seu aparelho.

## As abas do app

| Aba | O que tem |
|---|---|
| **Início** | Botão ATIVAR, status real (Shizuku, serviço, Acessibilidade, funções aplicadas, recusadas e não verificadas), aparelho reconhecido, perfis prontos |
| **Jogo** | Lista de jogos, motor, resolução e FPS, desempenho, toque e mira, contador |
| **Sistema** | Android Leve, Hz, memória, Google e WebView, e a seção **Ferramentas** |
| **Rede** | Rede de Partida, sinal agora e funções de internet |

Toda aba tem busca e o botão **Tudo**, que lista todas as funções.

## Funções em detalhe

### 🎮 Jogo
- **Modo de Jogo do Android e Hz da partida:** liga o modo de jogo do sistema e fixa a taxa de atualização certa enquanto você joga.
- **Resolução e FPS:** ajusta resolução e limite de FPS por jogo.
- **Driver de GPU atualizado / Caminho Gráfico:** escolhe o melhor caminho gráfico por jogo (inclusive ANGLE quando a GPU passa no teste).
- **Escudo Térmico:** reduz a carga antes de o celular frear por calor.
- **Espremer RAM:** libera memória antes da partida.
- **Detector de Travadas e Anti-Travadas:** encontra engasgos e prepara o jogo pra eles.
- **Fluidez VOID:** geração de quadros (Desligada / Auto / Leve) no perfil de cada jogo, no Android 14+.
- **Visão de Jogo:** 6 modos de tela sem mexer no DPI: Equilibrado, Competitivo, Cores Vivas, Visão no Escuro, Bateria Fria e Cor Real, com prévia.
- **Contador na Tela:** FPS em cima do jogo.

### 🧠 Motor VOID e IA VOID
- **Motor VOID:** lê a partida a cada 5 segundos (calor, bateria, FPS, RAM) e age antes do problema: chama o Escudo Térmico antes do freio e libera memória antes do engasgo.
- **IA VOID:** aprende **no seu próprio celular**, sem mandar nada pra internet, e prevê queda de FPS e subida de temperatura com 30 segundos de antecedência.
- **IA do Toque:** calibra a sensibilidade pelo Teste de Toque.

### 🫧 Balão VOID
Bolha roxa com um V sobre o jogo. Abre um painel com:
- FPS do jogo, Hz da tela, temperatura, bateria, RAM e ping ao vivo;
- **Liberar RAM** (ou segure o balão);
- **Comilões de RAM** com botão Parar;
- Não perturbe e relatório da partida.

### 📱 Sistema
- **Android Leve:** Doze, tarefas e sons do sistema mais leves no dia a dia.
- **Hz Adaptativo:** taxa alta quando precisa, baixa quando não precisa.
- **Perfil Automático e Lista de Congelamento:** apps que você escolhe ficam parados durante o jogo.
- **Analisador de Apps:** mostra o que pesa no celular.
- **Serviços Google e WebView:** reduz o peso deles enquanto você joga.
- **Cooperar com a Marca:** quando ligado, o VOID nunca desliga nem engana o motor de jogos da fabricante.

### 🌐 Rede
- **Rede de Partida:** prioriza Wi-Fi 5/6 GHz e mede ping, oscilação e perda.
- **Sem Internet no Jogo:** VPN **local** que bloqueia apps escolhidos durante a partida. Nada sai do celular.
- **Bluetooth Sem Atraso:** reduz atraso de fones Bluetooth.

## Ferramentas

| Ferramenta | Pra que serve |
|---|---|
| **Calor e Lentidão** | Diz por que o celular está quente ou lento agora: temperatura da bateria, CPU e GPU, freio por calor, apps que mais gastam, e o **Modo Fresco** com Desfazer |
| **Editor de Configurações** | Lê e edita configurações do sistema com 120 ajustes prontos, abas de Alteradas e Favoritas |
| **DNA VOID** | Receitas que aplicam vários ajustes de uma vez |
| **Módulos AxManager** | Instala e gerencia módulos com conferência do conteúdo, Raio-X e logs |
| **Scripts Brevent** | Roda scripts pela conexão Brevent e espera o fim de verdade |
| **Central Shizuku** | Verifica a conexão e corrige problemas comuns |
| **Modo Banco** | Mostra "o que o banco vê" e desliga o que faz app de banco reclamar |
| **Teste de Toque** | Mede a resposta da tela |
| **Labs** | Funções experimentais de desempenho, cada uma com o risco explicado |
| **Registro** | Histórico de tudo que o VOID fez |
| **Restaurar Tudo e Emergência** | Volta todas as configurações ao original |

## Permissões e por que cada uma é usada

| Permissão | Uso |
|---|---|
| Shizuku / AxManager | Mudar configurações do sistema (nível ADB) |
| Acessibilidade | Saber quando o jogo abre, sem ficar consultando o tempo todo |
| Serviço em 1º plano e notificações | Manter o motor vivo durante a partida |
| VPN | Só no **Sem Internet no Jogo**. É local: nenhum dado sai do celular |
| Sobreposição | Balão VOID, Contador na Tela e mira |
| Estatísticas de uso | Plano B quando a Acessibilidade está desligada |

O VOID **não tem anúncios, não coleta dados e não manda nada pra servidor**. A IA treina no próprio aparelho.

## Segurança: as regras do VOID

1. **Nada de chave inventada:** só comandos e configurações documentados ou confirmados.
2. **Chave da marca só é usada se já existe** no aparelho.
3. **O valor original é salvo antes** de qualquer mudança e devolvido depois.
4. **Sua mudança vence:** se você alterou algo depois do VOID, ele não sobrescreve.
5. **Seus módulos têm prioridade:** se um módulo controla uma configuração, o VOID não mexe nela.
6. **Nada pesado durante o jogo:** leituras e conferências acontecem antes ou depois.
7. **Resposta desconhecida = não mexe.**

## Como desfazer tudo

- Desligue o botão **ATIVAR**: as funções da partida param.
- **Restaurar Tudo** (Ferramentas): devolve cada configuração ao valor original salvo.
- **Emergência:** para tudo de uma vez se algo parecer errado.
- Desinstalar o VOID sem restaurar pode deixar alguma configuração alterada. Use Restaurar Tudo antes.

## Problemas comuns

| Problema | O que fazer |
|---|---|
| "Shizuku não está rodando" | Abra o Shizuku e inicie de novo (precisa depois de reiniciar o celular) |
| Uma tela mostra "Está demorando demais" | Toque pra tentar de novo. Se repetir, abra a **Central Shizuku** e toque em Corrigir |
| O Balão não aparece | Dê a permissão de **Sobreposição** ao VOID |
| O jogo não é detectado | Ligue a **Acessibilidade** do VOID ou dê **Estatísticas de uso** |
| App de banco reclamando | Use o **Modo Banco** |
| Celular esquentando | Abra **Calor e Lentidão** e use o **Modo Fresco** |
| Quero voltar ao normal | **Restaurar Tudo** |

## Perguntas frequentes

**Precisa de root?** Não.

**Pode dar ban no jogo?** O VOID mexe nas configurações do Android, não nos arquivos do jogo. Mesmo assim, cada jogo tem suas próprias regras: use por sua conta.

**Pode estragar o celular?** As mudanças são de configuração e reversíveis. O VOID salva o original e devolve com Restaurar Tudo.

**Gasta mais bateria?** Durante o jogo, algumas funções priorizam desempenho. Fora do jogo, o Android Leve e o Hz Adaptativo ajudam a economizar.

**Por que não está na Play Store?** O VOID usa acesso de nível ADB e muda configurações do sistema, o que as regras da loja limitam. Esta página é o canal oficial.

**É de graça?** Sim.

## Limitações conhecidas

- O Shizuku precisa ser iniciado de novo depois de cada reinício (sem root).
- Algumas marcas (Motorola, vivo/iQOO, Infinix/TECNO/itel, Huawei/Honor) não têm chave própria de Hz documentada; o VOID usa só as padrão do Android.
- Em Samsung, a chave de Hz da marca só é usada pra baixar a 60 Hz.
- A **Fluidez VOID** precisa do Android 14 ou mais novo.
- Resultados mudam de aparelho pra aparelho. Use o Antes e Depois pra medir no seu.

## Novidades

### 15.39.1
- **Calor e Lentidão** abre em cerca de 2 segundos, sem carregamento infinito.

### 15.39.0
- Telas não ficam mais presas em "Lendo…": depois de um erro ou 15 segundos aparece "toque pra tentar de novo".
- Leituras do Shizuku mais rápidas, até 4 ao mesmo tempo.
- Scripts Brevent, DNA VOID e Central Shizuku não travam mais.

### 15.38.0
- **Fluidez VOID**: geração de quadros por jogo (Desligada / Auto / Leve).

### 15.37.0 e anteriores
- Rede neural VOID que prevê queda de FPS e calor, Motor VOID, Balão VOID, Visão de Jogo 2.0, Modo Banco refeito e muito mais. Veja a página de [Releases](https://github.com/Ryuta290/VOID_ADB/releases).

## Verificar se o APK é oficial

| | |
|---|---|
| Pacote | `com.voidadb.gpu` |
| Versão | 15.39.1 (código 183) |
| SHA-256 do arquivo | `7e7d05632884d895b6f52d79b74039bf3547f53809696129be1f10e2982821ae` |
| Certificado de assinatura (SHA-256) | `62d78b78fb8e8c2a6c73fcb4990e5c4bcdfff8875a979b273b261370faba8531` |

Baixe só por aqui. Uma cópia com outro certificado **não é oficial** e o próprio VOID se recusa a rodar se for modificado.

## Direitos

© 2026 Pedro Zuki (VOID_ADB). Todos os direitos reservados.
O código-fonte não é público. É proibido redistribuir versões modificadas.
