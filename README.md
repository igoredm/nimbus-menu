# Nimbus Menu

A [Windhawk](https://windhawk.net) mod that replaces the Windows taskbar with a light dock, one per monitor, with its own Start menu.

**Site, with a demo you can try in the browser:** [nimbus.igoredm.com](https://nimbus.igoredm.com/)

![Dock and Start](https://raw.githubusercontent.com/igoredm/windhawk-mods/b8319aac0d112762c582a7a0b4778d6c1d72790a/start.png)

![Control center](https://raw.githubusercontent.com/igoredm/windhawk-mods/1635432cdfe302469b8963916e776999508ebee7/2.0-central.png)

## Install

1. Install [Windhawk](https://windhawk.net).
2. In Windhawk, open **Explore**, search for **Nimbus Menu** and click **Install**.

In 1.1 (the version on Windhawk today) the settings are on the mod's page in Windhawk (**Settings** tab). From 2.0 on, Nimbus has its own settings window: right-click the dock → **Settings**. The first time, a guided setup asks a few questions; you can change everything later in the settings.

## Versions

### 2.0.0: awaiting Windhawk's approval ([follow the review](https://github.com/ramensoftware/windhawk-mods/pull/7752))

Adds the status area, a control center, a player and notifications of its own.

- **Status area:** clock and calendar, volume (with each app's own), network and Wi‑Fi, battery, keyboard language.
- **Control center:** do not disturb, Bluetooth, night light, shortcuts, each monitor's brightness, sound and power. Each item opens its full panel inside it.
- **Each item where you want it:** on the dock, in the control center, in Start, in several places at once, or off.
- **Player:** whatever any app is playing, with cover, controls and that app's volume. On the dock as cover and title, cover only, title only, bars that move with the sound, or an icon.
- **Nimbus notifications:** cards in the corner you choose and a list by time; Win+N can open it. 15 sounds (or the Windows one), one for alerts and one for reminders.
- **Tray:** the icons of background apps, behind one button, side by side, in a grid or a list. Middle-click pins, dragging reorders.
- **Bluetooth:** turn it on and off, paired devices with their battery, connect and disconnect headphones and speakers.
- **Devices:** battery of wireless headphones, mice and controllers, with a warning at 20% and 10%.
- **Notes, reminders and the shelf** (drop files on the dock to keep them for a while).
- **Smarter search:** ignores accents, finds by initials ("vsc" finds VS Code), forgives typos, knows nicknames ("cmd") and puts what you use most first.
- **Complete sound panel (optional):** the apps playing on the left and every output on the right. Drag an app onto an output to play it there too, from one output to another to move it, × to take it off one; pick the default output and the one for calls.
- **Its own settings window** with a live preview, and a **guided setup**.
- Keyboard in Start, power options with a confirmation, high contrast and reduced animations followed.

![Player](https://raw.githubusercontent.com/igoredm/windhawk-mods/1635432cdfe302469b8963916e776999508ebee7/2.0-player.png)

![Search with a typo](https://raw.githubusercontent.com/igoredm/windhawk-mods/1635432cdfe302469b8963916e776999508ebee7/2.0-busca.png)

![Complete sound panel](https://raw.githubusercontent.com/igoredm/windhawk-mods/9fce5f4a3e282a33e0cc07cf228b5584a243caa1/2.0-som.png)

![Guided setup](https://raw.githubusercontent.com/igoredm/windhawk-mods/1635432cdfe302469b8963916e776999508ebee7/2.0-guiado.png)

### 1.1.0: Nov 18, 2026 (published on Windhawk)

- A Downloads tab in Start, with the newest files from the internet.
- Text selection and Ctrl+A/C/X/V in the search box.
- Right-click on files: open, open file location, copy path. End task in the dock's app menu.
- A more reliable Windows key; apps like Steam pinned with the right program.
- Without Windows' transparency (or with battery saver on), the glass turns into a solid color.

### 1.0.0: Nov 15, 2026

- The dock (floating or full width, 4 looks, zoom, live previews) and its own Start, with app, file and settings search.
- The Windows key opens Nimbus' Start; Ctrl+Esc still opens the Windows one.
- Settings for each monitor.

## Help and suggestions

- **Something isn't working?** [Ask for help](../../issues/new?template=help.yml)
- **An idea to make it better?** [Suggest it](../../issues/new?template=suggestion.yml)

Before asking, take a look at the [open and closed issues](../../issues?q=is%3Aissue): someone may have had the same problem.

### Getting a log

A log shows what the mod was doing, and helps a lot with bugs.

1. In Windhawk, open **Nimbus Menu** → **Advanced** tab → **Debug logging**: turn it on.
2. Download [DebugView](https://learn.microsoft.com/sysinternals/downloads/debugview) (from Microsoft) and open it.
3. Do what causes the problem.
4. Copy the lines that have `nimbus-menu` and paste them in your issue.

Turn debug logging off again when you're done.

## What it changes in Windows

With "Hide the Windows taskbar" on (the default), the whole Windows taskbar is hidden; from 2.0 on, Nimbus brings back its tray, clock and quick settings. A few of Nimbus' actions are Windows settings:

| What | When | How it comes back |
|---|---|---|
| The taskbar's own "Automatically hide the taskbar" option | While "Hide the Windows taskbar" is on, so the hidden taskbar doesn't reserve screen space | Your original choice is put back when the mod stops, on sign-out or shutdown, and at the next start after a crash. |
| Each app's "Show notification banners" switch (2.0) | Only if you turn on "Hide Windows' own banners" and confirm (off by default) | Every app's original value is saved first, and put back when the option goes off or the mod stops. |
| Night light, power plan, brightness, Bluetooth, Wi‑Fi, volume, keyboard language (2.0) | Only when you click them, like in Windows' quick settings | They're your choices, so they stay as you set them. |
| The default sound output, the one for calls, and each app's output (2.0, complete sound panel only, off by default) | Only when you drag an app or click Default or Calls. It uses the same parts of Windows its Sound settings use, which Microsoft doesn't document | Windows keeps them, as in Settings › Sound › Volume mixer. An app on a second output is a copy Nimbus plays while it runs. Going back to the simple panel puts it all back. |

**BatteryHub** (2.0, optional, off by default): with "Devices: use BatteryHub" on, Nimbus runs [BatteryHub](https://github.com/krisgfx9/Wireless-Device-Battery-Monitor) (installed separately) hidden every 5 minutes, only to read the batteries of USB receivers; it closes by itself.

If the Windows taskbar ever stays hidden, turn the mod off or restart Explorer.

---

## Português

Mod do [Windhawk](https://windhawk.net) que troca a barra de tarefas do Windows por uma dock leve, uma por monitor, com Iniciar próprio.

**Site, com uma demonstração pra testar no navegador:** [nimbus.igoredm.com](https://nimbus.igoredm.com/)

### Instalar

1. Instale o [Windhawk](https://windhawk.net).
2. No Windhawk, abra **Explore** (Explorar), busque **Nimbus Menu** e clique em **Install**.

Na 1.1 (a que está no Windhawk hoje), os ajustes ficam na página do mod no Windhawk (aba **Settings**). A partir da 2.0, o Nimbus tem janela de ajustes própria: botão direito na dock → **Ajustes**. Na primeira vez, um modo guiado faz umas perguntas; dá pra mudar tudo depois nos ajustes.

### Versões

**2.0.0: aguardando aprovação do Windhawk** ([acompanhar a revisão](https://github.com/ramensoftware/windhawk-mods/pull/7752))

Traz a área de status, uma central de controle, um player e notificações próprias.

- **Área de status:** relógio e calendário, volume (com o de cada app), rede e Wi‑Fi, bateria, idioma do teclado.
- **Central de controle:** não perturbe, Bluetooth, luz noturna, atalhos, brilho de cada monitor, som e energia. Cada item abre o painel completo dentro dela.
- **Cada item onde você quiser:** na dock, na central, no Iniciar, em vários lugares ao mesmo tempo, ou desligado.
- **Player:** o que qualquer app estiver tocando, com capa, controles e o volume do app. Na dock como capa e título, só capa, só título, barras que dançam com o som, ou ícone.
- **Notificações do Nimbus:** cartões no canto que você escolher e uma lista por horário; Win+N pode abrir. 15 sons (ou o do Windows), um pros avisos e outro pros lembretes.
- **Bandeja:** os ícones dos apps em segundo plano, num botão, lado a lado, em grade ou lista. Botão do meio fixa, arrastar reordena.
- **Bluetooth:** ligar e desligar, aparelhos pareados com bateria, conectar e desconectar fones e caixas.
- **Dispositivos:** bateria de fones, mouses e controles sem fio, com aviso em 20% e 10%.
- **Notas, lembretes e a prateleira** (solte arquivos na dock pra guardar por um tempo).
- **Busca mais esperta:** ignora acentos, acha por iniciais ("vsc" acha o VS Code), perdoa erro de digitação, conhece apelidos ("cmd") e põe o que você mais usa primeiro.
- **Painel de som completo (opcional):** os apps tocando à esquerda e todas as saídas à direita. Arraste um app pra uma saída pra tocar nela também, de uma saída pra outra pra trocar, × pra tirar de uma; escolha a saída padrão e a das chamadas.
- **Janela de ajustes própria** com prévia ao vivo, e **modo guiado**.
- Teclado no Iniciar, opções de energia com confirmação, alto contraste e "reduzir animações" do Windows respeitados.

**1.1.0: 18 nov. 2026 (publicada no Windhawk)**

- Aba Baixados no Iniciar, com os arquivos mais novos vindos da internet.
- Seleção de texto e Ctrl+A/C/X/V na busca.
- Botão direito em arquivos: abrir, abrir o local, copiar caminho. Finalizar tarefa no menu dos apps da dock.
- Tecla Windows mais confiável; apps como a Steam fixados com o programa certo.
- Sem a transparência do Windows (ou com a economia de bateria ligada), o vidro vira cor sólida.

**1.0.0: 15 nov. 2026**

- A dock (flutuante ou barra inteira, 4 visuais, zoom, prévias ao vivo) e o Iniciar próprio, com busca de apps, arquivos e configurações.
- A tecla Windows abre o Iniciar do Nimbus; Ctrl+Esc continua abrindo o do Windows.
- Ajustes por monitor.

### Ajuda e sugestões

- **Algo não está funcionando?** [Peça ajuda](../../issues/new?template=help.yml)
- **Uma ideia pra melhorar?** [Mande a sugestão](../../issues/new?template=suggestion.yml)

Antes de pedir, dê uma olhada nos [pedidos abertos e fechados](../../issues?q=is%3Aissue): alguém pode ter tido o mesmo problema.

### Como pegar o log

O log mostra o que o mod estava fazendo e ajuda muito a achar bugs.

1. No Windhawk, abra o **Nimbus Menu** → aba **Advanced** → **Debug logging**: ligue.
2. Baixe o [DebugView](https://learn.microsoft.com/sysinternals/downloads/debugview) (da Microsoft) e abra.
3. Faça o que causa o problema.
4. Copie as linhas que têm `nimbus-menu` e cole no seu pedido.

Depois desligue o debug logging de novo.

### O que muda no Windows

Com "Esconder a barra do Windows" ligado (o padrão), a barra do Windows some inteira; a partir da 2.0, o Nimbus traz de volta a bandeja, o relógio e as configurações rápidas. Algumas ações do Nimbus são configurações do Windows:

| O quê | Quando | Como volta |
|---|---|---|
| A opção "Ocultar automaticamente a barra de tarefas" do próprio Windows | Enquanto "Esconder a barra do Windows" estiver ligado, pra barra escondida não reservar espaço | A sua escolha original volta quando o mod para, ao sair da conta ou desligar, e no próximo início depois de um travamento. |
| O botão "Mostrar faixas de notificação" de cada app (2.0) | Só se você ligar "Esconder os avisos do Windows" e confirmar (desligado por padrão) | O valor original de cada app é salvo antes, e volta quando a opção é desligada ou o mod para. |
| Luz noturna, plano de energia, brilho, Bluetooth, Wi‑Fi, volume, idioma do teclado (2.0) | Só quando você clica, como nas configurações rápidas do Windows | São escolhas suas e ficam como você deixou. |
| A saída de som padrão, a das chamadas e a de cada app (2.0, só no painel de som completo, desligado por padrão) | Só quando você arrasta um app ou clica em Padrão ou Chamadas. Usa as mesmas partes do Windows que as Configurações de som usam, que a Microsoft não documenta | O Windows guarda, como em Configurações › Som › Mixer de volume. Um app numa segunda saída é uma cópia que o Nimbus toca enquanto roda. Voltar pro painel simples desfaz tudo. |

**BatteryHub** (2.0, opcional, desligado por padrão): com "Dispositivos: usar o BatteryHub" ligado, o Nimbus roda o [BatteryHub](https://github.com/krisgfx9/Wireless-Device-Battery-Monitor) (instalado à parte) escondido a cada 5 minutos, só pra ler a bateria de receptores USB; ele fecha sozinho.

Se a barra do Windows ficar escondida, desligue o mod ou reinicie o Explorador.
