# Test-dmd-Jupiter
このコードは試しに以下の木星の220枚の画像をpyDMD(https://github.com/PyDMD/PyDMD)で動かしたものです。

Jupiter Cloud Sequence from Cassini

https://svs.gsfc.nasa.gov/3610/

https://svs.gsfc.nasa.gov/vis/a000000/a003600/a003610/frames/3601x1801_2x1_30p/


データセットはターミナルで以下のようにダウンロードします。
mkdir -p ~/data/cassini_jupiter_tif
cd ~/data/cassini_jupiter_tif

wget -r -np -nd -A "*.tif" \
https://svs.gsfc.nasa.gov/vis/a000000/a003600/a003610/frames/3601x1801_2x1_30p/

以下のインストール必要です。
pip install pydmd
conda install -c conda-forge ffmpeg
