# Singleton CDI - Quarkus
## Resposta
Ao atribuir o parâmetro newConfig à this.config foi criado um novo objeto quando acessada
a segunda classe.

Por exemplo, foi acessado o ConfigResource pelo Swagger e alterado o formato do relatório
e também o tipo de Gráfico pelo PUT. 
Quando foi solicitado o GET, ainda do ConfigResourse, foi confirmada a mudança.

Porém, ao solicitar o GET do RelatorioResourse foi criado um novo objeto com os parâmetros iniciais.
Ou seja, o padrão singleton não estava mais funcionando.