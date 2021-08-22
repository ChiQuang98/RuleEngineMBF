docker build -t chiquang98/ruleenginembfimage .
docker save chiquang98/ruleenginembfimage  | gzip > ruleenginembfimage.tar.gz
zcat ruleenginembfimage.tar.gz | docker load
