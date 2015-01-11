# networkx_for_unicode
This is for unicode label.

## Modified files
networkx-1.9.1/networkx/drawing/nx_pylab.py

## Usage
```python
import matplotlib.font_manager as fm
# fp1 = fm.FontProperties(fname="./NanumGothic.otf")
fp1 = fm.FontProperties(fname="./NotoSansKR-Regular.otf") # Free Font https://www.google.com/get/noto/pkgs/NotoSansKorean-windows.zip
nx.set_fontproperties(fp1)
G = nx.Graph()
G.add_edge(u'한국어',u'영어')
nx.draw(G, with_labels=True)
```
