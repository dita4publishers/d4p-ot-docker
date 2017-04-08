FROM dita4publishers/dita-ot-common:1.8.5
#
# Sets up a DITA-OT container
# with all of the DITA for Publishers 
# open toolkit plugins integrated.
WORKDIR ${DITA_HOME}
ENV DITA_COMM_URL=https://github.com/dita4publishers/ BRANCH=develop
#
# Legacy sourceforge doctypes support:
#
RUN wget ${DITA_COMM_URL}net.sourceforge.dita4publishers.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/net.sourceforge.dita4publishers.doctypes-${BRANCH} plugins/net.sourceforge.dita4publishers.doctypes && rm ${BRANCH}.zip
#
# All plugins 
#
RUN wget ${DITA_COMM_URL}org.dita4publishers.dita2indesign/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.dita2indesign-${BRANCH} plugins/org.dita4publishers.dita2indesign && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.doctypes-${BRANCH} plugins/org.dita4publishers.doctypes && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.enumeration-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.enumeration-d.fo-${BRANCH} plugins/org.dita4publishers.enumeration-d.fo && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.enumeration-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.enumeration-d.html-${BRANCH}  plugins/org.dita4publishers.enumeration-d.html && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.epub/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.epub-${BRANCH} plugins/org.dita4publishers.epub && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.formatting-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.formatting-d.fo-${BRANCH} plugins/org.dita4publishers.formatting-d.fo && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.formatting-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.formatting-d.html-${BRANCH} plugins/org.dita4publishers.formatting-d.html && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.graphviz/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.graphviz-${BRANCH} plugins/org.dita4publishers.graphviz && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.html2/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.html2-${BRANCH} plugins/org.dita4publishers.html2 && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.html5/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.html5-${BRANCH} plugins/org.dita4publishers.html5 && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.json/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.json-${BRANCH} plugins/org.dita4publishers.json && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.kindle/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.kindle-${BRANCH} plugins/org.dita4publishers.kindle && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.math/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.math-${BRANCH} plugins/org.dita4publishers.math && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.pubContent-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.pubContent-d.fo-${BRANCH} plugins/org.dita4publishers.pubContent-d.fo  && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.pubmap.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.pubmap.fo-${BRANCH} plugins/org.dita4publishers.pubmap.fo && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.pubmap.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.pubmap.html-${BRANCH} plugins/org.dita4publishers.pubmap.html && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.rss/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.rss-${BRANCH} plugins/org.dita4publishers.rss && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.ruby.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.ruby.fo-${BRANCH} plugins/org.dita4publishers.ruby.fo && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.ruby.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.ruby.html-${BRANCH} plugins/org.dita4publishers.ruby.html && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.word2dita/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.word2dita-${BRANCH} plugins/org.dita4publishers.word2dita && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.xmldomain.doctypes-${BRANCH} plugins/org.dita4publishers.xmldomain.doctypes && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.xmldomain.fo-${BRANCH} plugins/org.dita4publishers.xmldomain.fo && rm ${BRANCH}.zip && \ 
wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && mv plugins/org.dita4publishers.xmldomain.html-${BRANCH} plugins/org.dita4publishers.xmldomain.html && rm ${BRANCH}.zip && \
#
# Integrate new plugins
#
ant -f integrator.xml
#
# End of Dockerfile
#

