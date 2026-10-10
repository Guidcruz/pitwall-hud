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
   **Executar assim mesmo**.
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
programa sem assinatura paga e não aceita exceção para um programa só, então o PitWall HUD não instala com ele ligado.
A opção fica em Segurança do Windows → Controle de aplicativos e do navegador; desligar ou não é decisão sua.

---

## How to install

1. From the [latest release](https://github.com/Guidcruz/pitwall-hud/releases/latest), under *Assets*, download
   `PitWallHUD-Setup-<version>.exe`.
2. If your browser says the file isn't commonly downloaded, choose **Keep**.
3. Open it. If **"Windows protected your PC"** shows up, click **More info**, then **Run anyway**.
4. The installer doesn't ask for admin rights: it installs for your user only. The app downloads and installs later
   versions by itself, outside of races (About → Update automatically, on by default).

**Why the warning?** PitWall HUD is free and has no code-signing certificate, which costs money every year. Without
one, Windows shows "Unknown publisher" for any program it doesn't know well yet. It doesn't mean Windows found anything
wrong with the file.

**Check the file (optional):** each release lists the installer's SHA-256 (same as the `.sha256` file). In PowerShell,
`Get-FileHash .\PitWallHUD-Setup-0.1.0.exe` must show the same hash.

**Blocked, no "Run anyway"?** Windows 11 **Smart App Control** is on. It blocks every program without a paid signature
and allows no per-app exception, so PitWall HUD can't be installed while it's on. The setting is in Windows Security →
App & browser control; turning it off is your call.
