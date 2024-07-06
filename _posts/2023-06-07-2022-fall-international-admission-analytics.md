---
layout: post
title: "2022年秋季US国际学生数据分析"
date: 2023-06-07
---
2022年秋季，美国的国际学生数量跟2021年对比有哪些变化呢？

ICE（US Immigration and Customs Enforcement）最近发布的SEVIS数据报告中，详细的列出了2022年秋季入学的各个学生群组（从K-12到博士项目）的国际学生数量。下面，我们一起从入学学生数量、专业和学校分布等角度来了解国际学生的情况。

如果你想了解美国2021年秋季『研究生』录取状况，请阅读我们之前的文章[美国2021秋季研究生录取数据分析](https://tessay.org/blog/2023/05/01/2021-fall-graduate-admission-statistics)。

**整体变化**

2019-2021年，受到covid影响，美国的国际学生数量出现了罕见的下降趋势。而随着全球covid情况缓解，2022年美国的国际学生数量回归增长趋势。2022年，持有F-1和M-1学生签证的总数是1,362,157，比2021年（1,236,748）增长10%，比2020年（1,251,569）增长8.8%。各类学生的具体比例和跟去年对比的变化是：

+ 33%的国际学生就读于本科项目（450,408）， 学生数量比2021年增长1.6%

+ 37%的国际学生就读于硕士项目（507,195），学生数量比2021年增加16%

+ 14%的学生就读于博士项目（197,183），学生数量比2021年增加了3.2% 

+ 5.2%的学生就读于副学士项目（associate degrees，71,445），学生数量比2021年增长2.8%

+ 3.9%的学生就读于K-12学校（53,751），学生数量比2021年增加8.3%


图1（Figure 1）中，我们对比了过去三年不同学生群体中国际学生数量。对比于2021年，2022年每类学生群体中的国际学生数量都有所增加，其中较为显著的是硕士项目。随着covid影响的减弱，2022年的本科、硕士和博士项目的学生数量高于2020年。


    
![png](/assets/images/2023-06-07-2022-fall-international-admission-analytics_files/2023-06-07-2022-fall-international-admission-analytics_3_0.png)
    


**最受国际学生欢迎的专业**

在接受高等教育的国际学生里，那些专业最受欢迎呢？

2022年，整体上国际学生就读于1485个专业，而其中最受欢迎的20个专业如下，包括Computer Science, Second Language Learning (英语之外的另一门语言), Business Administration and Management, Computer and Information Science, Electrical and Electronics Engineering等。就读于这20个专业(Figure 2)的学生数量占国际学生总数的50%。


    
![png](/assets/images/2023-06-07-2022-fall-international-admission-analytics_files/2023-06-07-2022-fall-international-admission-analytics_5_0.png)
    


**国际学生最多的学校**

美国学校中，国际学生最多的学校有哪些呢？

2022年，F-1国际学生就读的美国学校的总数为6432所。其中国际学生最多的前20所学校均为高等院校，包括 (Figure 3)：


    
![png](/assets/images/2023-06-07-2022-fall-international-admission-analytics_files/2023-06-07-2022-fall-international-admission-analytics_7_0.png)
    


**中国学生**

中国学生的数量有哪些变化呢？

中国学生占所有国际学生的比重最大，24% （324,196）。与2021年相比，2022年持有学生签证的中国学生数量降低了7.1%。2019-2022年中国学生数量整体呈现下降趋势，2021-2022下降趋势有所缓解，如图4 (Figure 4)。与此同时，另一个比较大的国际学生生源国印度的学生数量2020-2022年成上涨趋势，2022年学生数量为297,151。


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    File /opt/conda/lib/python3.11/site-packages/IPython/core/formatters.py:343, in BaseFormatter.__call__(self, obj)
        341     pass
        342 else:
    --> 343     return printer(obj)
        344 # Finally look for special method names
        345 method = get_real_method(obj, self.print_method)


    File /opt/conda/lib/python3.11/site-packages/IPython/core/pylabtools.py:152, in print_figure(fig, fmt, bbox_inches, base64, **kwargs)
        149     from matplotlib.backend_bases import FigureCanvasBase
        150     FigureCanvasBase(fig)
    --> 152 fig.canvas.print_figure(bytes_io, **kw)
        153 data = bytes_io.getvalue()
        154 if fmt == 'svg':


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backend_bases.py:2193, in FigureCanvasBase.print_figure(self, filename, dpi, facecolor, edgecolor, orientation, format, bbox_inches, pad_inches, bbox_extra_artists, backend, **kwargs)
       2189 try:
       2190     # _get_renderer may change the figure dpi (as vector formats
       2191     # force the figure dpi to 72), so we need to set it again here.
       2192     with cbook._setattr_cm(self.figure, dpi=dpi):
    -> 2193         result = print_method(
       2194             filename,
       2195             facecolor=facecolor,
       2196             edgecolor=edgecolor,
       2197             orientation=orientation,
       2198             bbox_inches_restore=_bbox_inches_restore,
       2199             **kwargs)
       2200 finally:
       2201     if bbox_inches and restore_bbox:


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backend_bases.py:2043, in FigureCanvasBase._switch_canvas_and_return_print_method.<locals>.<lambda>(*args, **kwargs)
       2039     optional_kws = {  # Passed by print_figure for other renderers.
       2040         "dpi", "facecolor", "edgecolor", "orientation",
       2041         "bbox_inches_restore"}
       2042     skip = optional_kws - {*inspect.signature(meth).parameters}
    -> 2043     print_method = functools.wraps(meth)(lambda *args, **kwargs: meth(
       2044         *args, **{k: v for k, v in kwargs.items() if k not in skip}))
       2045 else:  # Let third-parties do as they see fit.
       2046     print_method = meth


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backends/backend_agg.py:497, in FigureCanvasAgg.print_png(self, filename_or_obj, metadata, pil_kwargs)
        450 def print_png(self, filename_or_obj, *, metadata=None, pil_kwargs=None):
        451     """
        452     Write the figure to a PNG file.
        453 
       (...)
        495         *metadata*, including the default 'Software' key.
        496     """
    --> 497     self._print_pil(filename_or_obj, "png", pil_kwargs, metadata)


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backends/backend_agg.py:445, in FigureCanvasAgg._print_pil(self, filename_or_obj, fmt, pil_kwargs, metadata)
        440 def _print_pil(self, filename_or_obj, fmt, pil_kwargs, metadata=None):
        441     """
        442     Draw the canvas, then save it using `.image.imsave` (to which
        443     *pil_kwargs* and *metadata* are forwarded).
        444     """
    --> 445     FigureCanvasAgg.draw(self)
        446     mpl.image.imsave(
        447         filename_or_obj, self.buffer_rgba(), format=fmt, origin="upper",
        448         dpi=self.figure.dpi, metadata=metadata, pil_kwargs=pil_kwargs)


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backends/backend_agg.py:383, in FigureCanvasAgg.draw(self)
        381 def draw(self):
        382     # docstring inherited
    --> 383     self.renderer = self.get_renderer()
        384     self.renderer.clear()
        385     # Acquire a lock on the shared font cache.


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backends/backend_agg.py:398, in FigureCanvasAgg.get_renderer(self)
        396 reuse_renderer = (self._lastKey == key)
        397 if not reuse_renderer:
    --> 398     self.renderer = RendererAgg(w, h, self.figure.dpi)
        399     self._lastKey = key
        400 return self.renderer


    File /opt/conda/lib/python3.11/site-packages/matplotlib/backends/backend_agg.py:70, in RendererAgg.__init__(self, width, height, dpi)
         68 self.width = width
         69 self.height = height
    ---> 70 self._renderer = _RendererAgg(int(width), int(height), dpi)
         71 self._filter_renderers = []
         73 self._update_methods()


    ValueError: Image size of 5313x630000115 pixels is too large. It must be less than 2^16 in each direction.



    <Figure size 600x600 with 1 Axes>


**地理分布**

美国各地区中，2022年国际学生数量都比2021年有所增长，其中东北部增长11.6%，中西部增长11.5%，南部11%，西部8.3%。东北部国际学生数量最高，占美国国际学生总数的29.7%，其次是南部（28.1%）和西部（25.9%）。

所有州中，国际学生数量最高的五个州是California (16.8%), New York (11.5%), Texas (7.5%),  Massachusetts (7.2%), 和Florida (5.7%)。


**OPT**

图5（Figure 5）中我们看到，2019-2021年，通过OPT在美国工作的国际学生数量呈下降趋势，2022年，学生数量有所回升。2022年，有117,301位OPT学生拿到了工卡并在美国工作，比2021年（105,970）增加了10.7%。




    
![png](/assets/images/2023-06-07-2022-fall-international-admission-analytics_files/2023-06-07-2022-fall-international-admission-analytics_11_0.png)
    



以上就是2022年美国国际学生数量的数据分析。希望这篇文章能够对你的留学决定、专业和学校选择有帮助。

**References：**

+ https://www.ice.gov/doclib/sevis/pdf/sevisBTN2022.pdf

+ https://www.ice.gov/doclib/sevis/pdf/sevisBTN2021.pdf

+ https://www.ice.gov/doclib/sevis/pdf/sevisBTN2020.pdf

+ https://www.ice.gov/doclib/sevis/pdf/sevisBTN2019.pdf



