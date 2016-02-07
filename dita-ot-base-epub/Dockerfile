FROM ditacommunity/dita-ot-base:1.8.5
#
# Sets up a DITA-OT container
# with all of the DITA for Publishers 
# open toolkit plugins integrated.
USER dita-ot
WORKDIR ${DITA_HOME}
ENV DITA_COMM_URL=https://github.com/dita4publishers/ BRANCH=develop
#
# Legacy sourceforge doctypes support:
#
RUN wget ${DITA_COMM_URL}net.sourceforge.dita4publishers.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
#
# Legacy sourceforge doctypes support:
#
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.mapdriven/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.xslfo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.xslt/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.dita2indesign/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.enumeration-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.enumeration-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.epub/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.formatting-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.formatting-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.graphviz/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.html2/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.html5/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.json/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.kindle/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.math/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.math-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.media-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.pubContent-d.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.pubmap.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.pubmap.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.rss/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.ruby.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.ruby.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.sample.epub_override/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.word2dita/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.doctypes/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.fo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.xmldomain.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.example.d4p.epub-custom/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.example.d4p.html2extensions/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.example.d4p.word2ditaextension/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
#
# Integrate new plugins
#
RUN ant -f integrator.xml
#
# End of Dockerfile
#

