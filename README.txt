docker build -t chiquang98/ruleenginembfimage .
docker save chiquang98/ruleenginembfimage  | gzip > ruleenginembfimage.tar.gz
zcat ruleenginembfimage.tar.gz | docker load
docker run -p 8000:8000 -d dockerimageid
