FROM alpine

WORKDIR	 /app

COPY 1 2/

RUN echo "问:什么单词以 R 开头且没有结尾? 答:重组(Reorganization)。 " > /app/2/2.txt

RUN cat /app/2/2.txt
RUN cat /app/2/1.txt
ENV AE=86  AK=47
RUN echo $AE, $AK

EXPOSE 333

VOLUME /app/data

CMD echo  $AK