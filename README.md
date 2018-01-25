
# PLUGIN SETUP

```
pip3 install pyflakes
pip3 install pycodestyle

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
git clone https://github.com/rdunklau/Gedit-checkpython.git

popd


pushd ~/Programs/
wget https://github.com/pmd/pmd/releases/download/pmd_releases%2F5.8.1/pmd-bin-5.8.1.zip
unzip pmd-bin-5.8.1.zip
rm pmd-bin-5.8.1.zip
mv pmd-bin* pmd-bin
popd

mkdir -p ~/.config/gedit/tools/
pushd ~/.config/gedit/tools/
git clone https://github.com/89luca89/gedit-external-tools-ide .
popd

git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
echo "alias s='fzf -x'
alias gs='fzf -x | xargs gedit'" >> ~/.bashrc

gsettings set org.gnome.gedit.plugins active-plugins "['docinfo', 'snippets', 'pythonconsole', 'smartspaces', 'synctex', 'bracketcompletion', 'bookmarks', 'commander', 'multiedit', 'textsize', 'externaltools', 'filebrowser', 'colorschemer', 'findinfiles', 'terminal', 'latex', 'codecomment', 'git', 'quickopen', 'sort', 'colorpicker', 'drawspaces', 'joinlines', 'time', 'spell', 'modelines', 'wordcompletion', 'charmap', 'mdoutline', 'gracer', 'darktheme', 'multicursor', 'gtagJump', 'scroll_past', 'sourcecodebrowser', 'panel_toggler', 'controlyourtabs', 'reflow']"
```

