# Robots.txt

## Antes de começar

O Robots é um arquivo de configuração que é recomendado ficar no diretório raiz da aplicação , ele é responsável por conter uma listagem de diretórios e arquivos que os administradores não querem que sejam indexados pelos **Web Crawlers** como por exemplo:
- Google
- Bing

O arquivo **robots.txt** pode ser uma mina de ouro , pois nela podemos encontrar arquivos sensíveis , diretórios e que pode ser um perigo caso seja indexado pelos Crawlers.

Veja o exemplo do facebook
```sh
http://fatecbauru.edu.br/robots.txt
```

![Robots.txt](https://i.imgur.com/ZtQb5Wb.png)

Vamos realizar um teste agora em um grande site como o facebook para ver as diferenças
```sh
https://facebook.com/robots.txt
```

Diferente ?

## Vale a pena
Existem algumas coisas que precisamos prestar atenção , elas são

- Arquivos
- Diretórios
- PATHS
- Clean URLS
- No Clean URLS

### Arquivos
Esse tipo de arquivo sempre é bom analisar , se alguém não quer que seja indexado no google e porque pode ter algum valor.

### Diretorios ou PATHS
Diretórios ou caminhos também é valido analisar , em algum teste um analista pode precisar procurar uma área de administração , diretórios de upload e toda informação é valida.

### Clean URLS
Clean URLS são caminhos absolutos onde podemos copiar e colar em nosso navegador e acessar.

### No Clean URLS
No Clean URLS são caminhos que precisam de um parâmetro , muitas vezes utilizado para proporcionar uma função a mais.

## Recomendações
É recomendável que todo servidor web tenha um arquivo robots.txt em sua raiz , caso contrario todos os arquivos podem ser indexados pelos **web crawlers** e isso pode ser algo perigoso.

Pois arquivos , diretórios e até backups do banco de dados podem estar públicos na internet.

É recomendável que sempre tenha um arquivo **robots.txt** na raiz do seu servidor web , mais onde é a raiz ?

### No Linux
No sistema linux costumar estar em
```sh
 /var/www/
```

ou até
```sh
 /var/www/html/
```

### No Windows
```sh
C:/inetpub/wwwroot/
```
