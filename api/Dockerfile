FROM python

LABEL "com.project.author"="Walther" version="0.1"

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "uvicorn", "main:app" ]

EXPOSE 8000

# HEALTHCHECK --interval=5m --timeout=3s CMD curl -f http://localhost/ || exit 1
