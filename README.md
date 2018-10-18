# jasperreports-fonts
jasperreports-fonts

解决 jasperreports 无法显示中文的问题

新增自定义字体

在 fonts.xml 添加如下信息
~~~xml

<fontFamily name="宋体">
            <normal>net/sf/jasperreports/fonts/cn/STSONG.TTF</normal>
            <bold>net/sf/jasperreports/fonts/cn/STSONG.TTF</bold>
            <italic>net/sf/jasperreports/fonts/cn/STSONG.TTF</italic>
            <boldItalic>net/sf/jasperreports/fonts/cn/STSONG.TTF</boldItalic>
            <pdfEncoding>Identity-H</pdfEncoding>
            <pdfEmbedded>true</pdfEmbedded> <exportFonts>
                <export key="net.sf.jasperreports.html">'宋体', Arial, Helvetica, sans-serif</export>
                <export key="net.sf.jasperreports.xhtml">'宋体', Arial, Helvetica, sans-serif</export>
            </exportFonts>
            <!--
                <locales>
                    <locale>en_US</locale>
                    <locale>de_DE</locale>
                </locales>
            -->
        </fontFamily>
~~~

~~~xml
<fontFamily name="宋体">
        <exportFonts>
            <export key="net.sf.jasperreports.html">'宋体', Arial, Helvetica, sans-serif</export>
            <export key="net.sf.jasperreports.xhtml">'宋体', Arial, Helvetica, sans-serif</export>
        </exportFonts>
</fontFamily>

~~~