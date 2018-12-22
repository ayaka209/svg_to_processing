# svg_to_processing
a very simple web page to convert a svg to processing code


example: ( icon is from https://icons8.com/icon/set/cake/ios )
```
<svg version="1.0"  xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
     viewBox="0 0 800 800" style="enable-background:new 0 0 800 800;" xml:space="preserve">
<title>Birthday_Cake</title>
    <path style="fill:rgb(255,181,210);" d="M330,410V260c0-16.6,13.4-30,30-30h80c16.6,0,30,13.4,30,30v150H330z"/>
    <path style="fill:rgb(234,76,137);" d="M440,240c11,0,20,9,20,20v140H340V260c0-11,9-20,20-20H440 M440,220h-80c-22.1,0-40,17.9-40,40v160
	h160V260C480,237.9,462.1,220,440,220z"/>
    <rect x="70" y="510" style="fill:#DBB065;" width="660" height="180"/>
    <path style="fill:rgb(150,122,68);" d="M720,520v160H80V520H720 M740,500H60v200h680V500z"/>
    <path style="fill:rgb(255,255,255);" d="M100,770c-38.7,0-70-31.3-70-70v-10h740v10c0,38.7-31.3,70-70,70H100z"/>
    <path style="fill:rgb(120,139,156);" d="M760,700c0,33.1-26.9,60-60,60H100c-33.1,0-60-26.9-60-60H760 M780,680H20v20c0,44.2,35.8,80,80,80
	h600c44.2,0,80-35.8,80-80V680z"/>
    <path style="fill:rgb(255,196,156);" d="M630,590c-36.3,2.2-71.2-14.2-92.6-43.6l-7.6-13l-9,12c-20,26.6-68.4,44.6-120,44.6s-100-18-120-44.6
	l-9-12l-7.6,13c-21.7,29.9-57.4,46.4-94.2,43.6c-55.2,0-100-31.4-100-70v-20c0-49.7,40.3-90,90-90h480c49.7,0,90,40.3,90,90v20
	C730,558.6,685.2,590,630,590z"/>
    <path style="fill:rgb(161,106,74);" d="M640,420c44.2,0,80,35.8,80,80v20c0,32.6-41.2,60-90,60c-32.7,1.9-64.3-12.6-84-38.8l-15.2-26
	l-18,24.8c-15,20-55.8,40-112.8,40s-97.6-20-112.8-40l-18-24.2l-15.2,26c-19.9,25.9-51.4,40.3-84,38.2c-48.8,0-90-27.4-90-60v-20
	c0-44.2,35.8-80,80-80H640 M640,400H160c-55.2,0-100,44.8-100,100v20c0,44.2,49.2,80,110,80c39.8,2.2,78-16.1,101.2-48.6
	C292.6,580,342.2,600,400,600s107.4-20,128.8-48.6C552,583.9,590.2,602.2,630,600c60,0,110-35.8,110-80v-20
	C740,444.8,695.2,400,640,400z"/>
    <path style="fill:rgb(255,238,163);" d="M400,210c-38.7,0-70-31.3-70-70c0-29.8,45.2-92.8,70-124.2c24.8,31.4,70,94.4,70,124.2
	C470,178.7,438.7,210,400,210z"/>
    <path style="fill:rgb(186,155,72);" d="M400,32c28.6,37.4,60,86.4,60,108c0,33.1-26.9,60-60,60s-60-26.9-60-60C340,118.6,371.4,69.4,400,32
	 M400,0c0,0-80,95.8-80,140c0,44.2,35.8,80,80,80s80-35.8,80-80C480,95.8,400,0,400,0z"/>
    <path style="fill:rgb(199,67,67);" d="M430,170c0,16.6-13.4,30-30,30s-30-13.4-30-30c0-16.6,30-60,30-60S430,153.4,430,170z"/>
</svg>
```
based on: (they did 99% work)
- path-data-polyfill (MIT License) https://github.com/jarek-foksa/path-data-polyfill

which is based on
- SVGPathSeg polyfill by Philip Rogers (MIT License)
  https://github.com/progers/pathseg
- SVGPathNormalizer by Tadahisa Motooka (MIT License)
  https://github.com/motooka/SVGPathNormalizer/tree/master/src
- arcToCubicCurves() by Dmitry Baranovskiy (MIT License)
  https://github.com/DmitryBaranovskiy/raphael/blob/v2.1.1/raphael.core.js#L1837
