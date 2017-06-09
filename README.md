
# PLUGIN SETUP

```
mkdir -p ~/.local/share/gedit/plugins/
pushd ~/.local/share/gedit/plugins/

git clone https://github.com/guillaumechereau/gedit-reflow-plugin
git clone https://github.com/mikecrittenden/zen-coding-gedit
git clone https://github.com/isamert/gracer
git clone https://github.com/franzzapata/gedit-darktheme
git clone https://github.com/suniobo/gedit-markdown-outline
git clone https://github.com/hardpixel/gedit-panel-toggler
git clone https://github.com/jefferyto/gedit-control-your-tabs
git clone https://github.com/hardpixel/gedit-scroll-past
git clone https://github.com/dinkel/gedit-zoom
git clone https://github.com/jessecrossen/Gedit-MultiCursor
git clone https://github.com/toobaz/gedit-source-code-browser/
git clone https://github.com/utisam/gtagJump.git
https://github.com/pallabpain/code-autocomplete-gedit3
https://github.com/addiks/gedit-phpide

popd

mkdir -p ~/.config/gedit/tools/
pushd ~/.config/gedit/tools/
git clone https://github.com/89luca89/gedit-external-tools-ide .
popd

git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
echo "alias s='fzf'
alias gs='fzf | xargs gedit'" >> ~/.bashrc

wget https://raw.githubusercontent.com/ilogue/docker.lang/master/docker.lang -O  ~/.local/share/gtksourceview-3.0/language-specs/docker.lang


gsettings set org.gnome.gedit.plugins active-plugins "['textsize', 'git', 'charmap', 'terminal', 'filebrowser', 'pythonconsole', 'snippets', 'beesu', 'smartspaces', 'bookmarks', 'wordcompletion', 'codecomment', 'synctex', 'findinfiles', 'multiedit', 'quickopen', 'commander', 'drawspaces', 'time', 'colorpicker', 'externaltools', 'modelines', 'colorschemer', 'sort', 'joinlines', 'spell', 'zeitgeist', 'bracketcompletion', 'docinfo', 'scroll_past', 'gracer', 'sourcecodebrowser', 'panel_toggler', 'darktheme', 'auto-complete', 'addiks-phpide', 'mdoutline', 'multicursor', 'controlyourtabs', 'reflow', 'gtagJump']"
```

