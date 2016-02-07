FROM ditacommunity/dita-ot-base:2.2.2
#
# Sets up a DITA-OT container
# with all of the DITA for Publishers 
# open toolkit plugins integrated.
WORKDIR ${DITA_HOME}
ENV DITA_COMM_URL=https://github.com/dita4publishers/ BRANCH=develop
#
# Common plugins needed by all transforms:
#
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.mapdriven/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.xslfo/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.common.xslt/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.math-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
RUN wget ${DITA_COMM_URL}org.dita4publishers.media-d.html/archive/${BRANCH}.zip && unzip ${BRANCH}.zip -d plugins && rm ${BRANCH}.zip
#
# Integrate new plugins
#
RUN ant -f integrator.xml
#
# End of Dockerfile
#

