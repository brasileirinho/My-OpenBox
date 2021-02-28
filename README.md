<h1>INTRODUÇÃO</h1>
<p>
  Guia simplificado de configuração e customização do meu OpenBox (Bunsenlabs)
  Não sou especialista em Linux e sim um apaixonado que gosta de brincar, testar
  e aprender, portanto, provavelmente este guia terá alguns erros, nada que o
  nosso amigo Google não resolva. Aceito sugestões e dicas para melhorar o meu
  ambiente, lembrando que essas são as minhas configurações, fiz para o meu uso,
  fique a vontade para fazer mudanças em seu sistema estou apenas compartilhando
  os meus conhecimentos
</p>
<p>
  Depois de muitas tentativas com XFCE GNOME LXDE KDE I3WM enfim consegui
  encontrar o meu sistema e configuração perfeito, que melhor se adapta ao meu
  "estilo" (olha que demorou muito haha). A ideia inicial é um sistema leve
  rápido com aparência minimalista e grande produtividade, conseguindo tudo sem
  tirar as mãos do teclado.
</p>

<p>
  <b>DICAS:</b> Se quiser pode realizar essa personalização instalando o Debian minimal só ter certeza de que já possui alguns pacotes essenciais como Xorg, Display Manager, Sound Mixer, Network Manager, etc. Minha recomendação é começar com o Bunsenlabs é um sistema bem construido, apenas com programas e recusros essenciais.
</p>

<h1>O que vamos fazer ?</h1>
  <ul>
    <li>Personalizar painel ( cores, tamanho pisição, funcionalidades )</li>
    <li>Personalizar Menu ( deixando mais Limpo ) </li>
    <li>Personalizar Janaleas</li>
    <li>Atalhos no teclado para aumentar a produtividade ( tudo sem tirar as mãos do teclado )</li>
    <li>Personalizar Shell "terminal" com ZSH ( Oh my zsh )</li>
    <li>Aparencia do Sistema ( tema GTK Yeti e Papitus já existente no Bunsenlabs )</li>
    <li>Wallpaper editado por mim</li>
    <li>Instalação de alguns programas que utilizo ( Gimp, VsCode, Git, NVM, e Yarn )</li>
  </ul>

<h1>DOCUMENTAÇÃO</h1>
<p><b>Bunsenlabs:</b>https://www.bunsenlabs.org/</p>
<p><b>OpenBox:</b>http://openbox.org/wiki/Main_Page</p>
<p><b>OhMyZSH:</b>https://ohmyz.sh/</p>
<p><b>Forum:</b>https://www.vivaolinux.com.br/comunidade/OpenBox/forum/</p>

<h1>DIRETORIOS</h1>
<b>[.xbindkeysrc]</b>
<p>home/.xbindkeysrc</p>

<b>[autostart]</b>
<p>/home/bernal/.config/bunsen/autostart</p>

<b>[bl-rc.xml]</b>
<p>/home/bernal/.config/openbox/bl-rc.xml</p>

<b>[prepend.csv]</b>
<p>/home/bernal/.config/jgmenu/prepend.csv</p>

<b>[.zshrc]</b>
<p>/home</p>

<h1>ZSH - INSTALAÇÃO E COSTUMIZAÇAO</h1>
<h4>ZSH - Instalação e Costumização</h4>
<p>1. sudo apt install zsh</p>
<p>
  2. sh -c "$(curl -fsSL
  https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
</p>
<p>
  3.sh -c "$(curl -fsSL
  https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)" OBS:
  quando rodar o item 3 vai perguntar se você quer ou não instalar os plugins
  recomendados, excolher opção N (NÃO)
</p>
<p>
  4. git clone https://github.com/denysdovhan/spaceship-prompt.git
  "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
</p>
<p>
  5. ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme"
  "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
</p>

<p>
  6.Plugins (zsh-autosuggestions & zsh-syntax-highlighting) git clone
  https://github.com/zsh-users/zsh-autosuggestions.git
  $ZSH_CUSTOM/plugins/zsh-autosuggestions 
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
  $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
</p>
<p>7. copiar e colocar script .zshrc ( diretorio a cima)</p>

<h1>PROGRAMAS E UTILITÁRIOS</h1>
<b>Git - instalação</b>
sudo apt install git

<b>NVM - instalação</b>
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.0/install.sh |
$SHELL nvm install --lts

<b>YARN - instalação</b>
npm install --global yarn

<b>Gimp - Instalação</b>
sudo apt install gimp

<h1>Screenshot</h1>

<h4>Desktop e Wallpaper</h4>
<img src="Screenshot/desktop.png" />

<h4>Desempenho</h4>
<img src="Screenshot/desempenho.png" />

<h4>Terminal e ZSH</h4>
<img src="Screenshot/zsh.png" />

<h4>Painel</h4>
<img src="Screenshot/painel.png" />

<h4>Janelas (não utilizo a borda decorada então para fechar, minimizar e maximizar só pelo teclado ou terminal</h4>
<img src="Screenshot/janela.png" />



<h1>Atalhos Keyboard</h1>

<h2>*Janelas</h2>
<p><b>Fechar Janela:</b> WIN + 1</p>
<p><b>Maximizar Janela:</b> WIN + 2</p>
<p><b>Fechar Minimizar:</b> WIN + 3</p>
<p>
  <b>Mover janela:</b> WIN + cima ou WIN + baixo ou WIN + direita ou WIN +
  esquerda
</p>
<p>
  <b>Mover janela Bloco:</b> WIN + ALT + cima ou WIN + ALT + baixo ou WIN + ALT +
  direita ou WIN + ALT+ esquerda
</p>
<p><b>Mover janela com Mouse:</b> ALT + arrastar c/ Mouse</p>

<h2>*Programas</h2>
<p><b>Web:</b> WIN + W</p>
<p><b>Bloco de notas:</b> WIN + E</p>
<p><b>Spotify:</b> WIN + S</p>
<p><b>Arquivos:</b> WIN + F</p>
<p><b>Terminal:</b> WIN + T</p>
<p><b>Gimp:</b> WIN + G</p>
<p><b>Controle de Áudio:</b> WIN + V</p>
<p><b>Visual Studio Code:</b> WIN + C</p>

<h2>*Sistema</h2>
<p><b>Reiniciar, Desligar, Suspender, Hibernar:</b> WIN + X</p>
<p><b>Menu:</b> WIN</p>

<h3>Obrigado !</h3>

