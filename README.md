# Singleton CDI - Quarkus
## Resposta
Ao atribuir o parâmetro newConfig à this.config foi criado um novo objeto quando acessada
a segunda classe.
Por exemple foi aberta a classe ConfigResource pelo Swagger a alterado o formato do relatório
e também o tipo de Gráfico. 
Quando foi acessado o GET ainda do ConfigResourse foi confirmado a mudança.

Porém ao acessar o GET do RelatorioResourse foi criado um novo objeto. Ou seja, o padrão singleton
não estava mais funcionando.