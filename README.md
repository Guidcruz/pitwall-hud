# PitWall HUD

Overlays leves por cima de simuladores de corrida (começando pelo iRacing): Standings, Relative, Combustível,
Inputs, Sessão e clima, Delta, Radar e Mapa da pista.

**Site:** https://guiracing.app/pitwall-hud/ · **Download:** [última versão](https://github.com/Guidcruz/pitwall-hud/releases/latest)

Este repositório publica só os instaladores e as atualizações. O app confere cada atualização pelo SHA-256 publicado
junto (`.sha256`) antes de instalar.

## Como instalar

1. Na [última versão](https://github.com/Guidcruz/pitwall-hud/releases/latest), em *Assets*, baixe o
   `PitWallHUD-Setup-<versão>.exe`.
2. Se o navegador avisar que o arquivo não é baixado com frequência, escolha **Manter**.
3. Abra o arquivo. Se aparecer **"O Windows protegeu o computador"**, clique em **Mais informações** e depois em
   **Executar assim mesmo**. Se o Windows bloquear sem essa opção, veja
   [Bloqueado, sem "Executar assim mesmo"?](#bloqueado-sem-executar-assim-mesmo) abaixo.
4. O instalador não pede administrador: instala só para o seu usuário. As versões seguintes o próprio app baixa e
   instala, fora das corridas (Sobre → Atualizar automaticamente, que já vem ligado).

### Por que o Windows avisa?

O PitWall HUD é gratuito e não tem certificado de assinatura de código, que é pago todo ano. Sem ele, o Windows mostra
"Editor desconhecido" para qualquer programa que ainda conhece pouco. O aviso não quer dizer que o Windows encontrou
algo de errado no arquivo.

### Conferir o arquivo (opcional)

As notas de cada versão trazem o SHA-256 do instalador (o mesmo do arquivo `.sha256`). No PowerShell, na pasta do
download:

```powershell
Get-FileHash .\PitWallHUD-Setup-0.1.0.exe
```

O `Hash` tem de ser igual ao publicado (maiúsculas ou minúsculas, tanto faz).

### Bloqueado, sem "Executar assim mesmo"?

Então o **Controle Inteligente de Aplicativos** (Smart App Control) do Windows 11 está ligado. Ele bloqueia todo
programa sem assinatura paga e não aceita exceção para um programa só, então o PitWall HUD não instala nem abre com ele
ligado. É a mesma causa quando o app já está instalado, não abre e o Windows avisa "Parte deste aplicativo foi
bloqueado".

Para usar o PitWall HUD, desligue o Controle Inteligente de Aplicativos:

1. Abra **Segurança do Windows** (procure no menu Iniciar).
2. Entre em **Controle de aplicativos e do navegador** → **Configurações do Controle Inteligente de Aplicativos**.
3. Escolha **Desligado**.
4. Abra o instalador (ou o app) de novo.

O antivírus do Windows continua ligado; sai só essa verificação de assinatura. Nas versões recentes do Windows 11 dá
para religar na mesma tela; nas anteriores, a Microsoft só permitia religar reinstalando o Windows. Desligar ou não é
decisão sua.

---

## How to install

1. From the [latest release](https://github.com/Guidcruz/pitwall-hud/releases/latest), under *Assets*, download
   `PitWallHUD-Setup-<version>.exe`.
2. If your browser says the file isn't commonly downloaded, choose **Keep**.
3. Open it. If **"Windows protected your PC"** shows up, click **More info**, then **Run anyway**. If Windows blocks
   it with no such option, see **Blocked, no "Run anyway"?** below.
4. The installer doesn't ask for admin rights: it installs for your user only. The app downloads and installs later
   versions by itself, outside of races (About → Update automatically, on by default).

**Why the warning?** PitWall HUD is free and has no code-signing certificate, which costs money every year. Without
one, Windows shows "Unknown publisher" for any program it doesn't know well yet. It doesn't mean Windows found anything
wrong with the file.

**Check the file (optional):** each release lists the installer's SHA-256 (same as the `.sha256` file). In PowerShell,
`Get-FileHash .\PitWallHUD-Setup-0.1.0.exe` must show the same hash.

**Blocked, no "Run anyway"?** Windows 11 **Smart App Control** is on. It blocks every program without a paid signature
and allows no per-app exception, so PitWall HUD can't be installed or opened while it's on. Same cause when the app is
installed but won't open and Windows says "Part of this app has been blocked". To use PitWall HUD, turn it off:

1. Open **Windows Security** (search for it in the Start menu).
2. Go to **App & browser control** → **Smart App Control settings**.
3. Choose **Off**.
4. Open the installer (or the app) again.

Windows' antivirus stays on; only this signature check goes away. On recent Windows 11 versions you can turn it back on
in the same place; on earlier ones, Microsoft only allowed turning it back on by reinstalling Windows. It's your call.
