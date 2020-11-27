# Tutoriais do wiki da dsiciplina convertidos em Rmarkdown

1. Se houve atualizações no (http://cmq.esalq.usp.br/BIE5781/)[wiki da disciplina] abra a página do tutorial para edição no dokuwiki, copie todo o seu coneteúdo e grave nos arquivos que estão no ditetório dokuwiki. É um arquivo texto, mas usamos a extensão `.dokuwiki` só para organizar.
2. Para converter o arquivo texto copiado do wiki da disciplina para o formato markdown recomendamos o (https://pandoc.org/)[pandoc], com o comando, executado do diretório "dokuwiki":

```
pandoc -f dokuwiki -t markdown arquivo.dokuwiki > ../rmarkdown/arquivo.Rmd
```

Onde `arquivo.dokuwiki` é o nome do arquivo texto do tutorial copiado para o diretório "dokuwiki"

3. Neste arquivo convertido os *chunks* em R estarão iniciados com o marcador `{.rsplus}`. Faça uma busca substituição por `{r}`

4. Agora é verificar se todo o tutorial convertido para rmarkdown funciona e gera pdfs e htmls.
