FROM nginx:1.25

RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d
# RUN addgroup --system app && adduser --system --group app

ENV APP_HOME=/home/app/web

RUN mkdir -p $APP_HOME/staticfiles
RUN mkdir -p $APP_HOME/mediafiles
# RUN chown -R app:app $APP_HOME/
# WORKDIR $APP_HOME