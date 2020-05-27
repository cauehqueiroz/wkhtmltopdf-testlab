# wkhtmltopdf-testlab

Projeto para gerar PDFs baseados em HTML com o motor WebKit (wkhtmltopdf)

## Modo de usar

Para iniciar o serviço:

```
$ docker-compose up -d
```

Em seguida, após o serviço subir você pode chamar o comando pelo conteiner da seguinte maneira:

Teste com o HTML padrão que já está no repo:
```
$ docker exec wkserver wkhtmltopdf /app/default.html /app/output.pdf
```

Você pode usar outro arquivo ou alterar o arquivo de saída:

```
$ docker exec wkserver wkhtmltopdf /app/outro_arquivo.html /app/outra_saida.pdf
```