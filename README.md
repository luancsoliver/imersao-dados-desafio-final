![imagem do título](https://www.wreducacional.com.br/img_cursos/prod/img_1230x644/saude/farmacologia.jpg)

# Desenvolvendo um modelo para prever ativação dos inibidores NF-KB e Proteassoma

## Introdução

NF-KB é um complexo proteico que desempenha funções relacionadas com fator de transcrição. Ele é encontrado em quase todos os tipos de células animais e está envolvido com a resposta celular a estímulos de estresse. [mais informações clique aqui](https://pt.wikipedia.org/wiki/NF-%CE%BAB). NF-KB regulam vários processos fisiológicos importantes, incluindo inflamação e respostas imunológicas, crescimento celular, apoteose e a expressão de certos genes virais. Portanto, a via de sinalização NF-KB também forneceu um foco para intervenção farmacológica, principalmente em situações de inflamação crônica ou em câncer, onde a via é frequentemente constitutivamente ativa e desempenha um papel fundamental na doença. [acesse o artigo para mais informações](https://www.nature.com/articles/1209982.pdf).

Proteassoma é um complexo proteico responsável pela degradação de proteínas itracelulares desempenhando um papel central na homeostase proteica por regular diversos processos celulares. [mais informações clique aqui](http://redoxoma.iq.usp.br/paginas_view.php?idPagina=935#.YJfsJSZv81I). Ela é usada para destruir proteínas danificadas ou com erros de síntese, as quais são marcadas para degradação através da ligação de cadeias de [ubiquitina](https://pt.wikipedia.org/wiki/Ubiquitina) em série. É importante que a célula destrua essas proteínas pois elas são potencialmente perigosas. [mais informações clique aqui](https://pt.wikipedia.org/wiki/Proteassoma).

Os inibidores de proteassoma são uma classe importante de medicamentos para o tratamento de [mieloma múltiplo](https://www.abrale.org.br/doencas/mieloma-multiplo/o-que-e/) e [linfoma de células do manto](https://www.abrale.org.br/doencas/linfomas/lnh/subtipos/linfoma-do-manto/o-que-e/) e estão sendo investigados para outras doenças. Enquanto inibidores de NF-KB estão sendo estudados para tratamento de certos tipos de câncer e doenças neodegenerativas e inflamatórias. [acesse o artigo para mais informações](https://www.nature.com/articles/1209982.pdf).

## Fonte de Dados

Os dados usados neste projetos originaram do Laboratory innovation science at Harvard. Os dados foram levantados de 23.813 amostras onde foram testados 3.289 tipos de compostos que podem dar origem à fármacos. Obtiveram dados de expressão gênica de 772 genes e de viabilidade celular de 100 tipos celulares. A partir desses dados ele podem prever a reação do organismo aos compostos e criar diferentes tipos de drogas para uso de humanos.

Com os dados iniciais sobre o efeito dos compostos sobre os genes e células testou-se a ativação de 206 diferentes substâncias. É aqui que entra os inbidores de NF-KB e Proteassoma.

## Objetivos

Esse projeto visa mostrar a importância destes dois inibidores na farmacologia, mostrar como a ativação deles afeta culturas celulares e criar um modelo de Machine Learning que consegue prever a ativação destes inibidores com as informações genéticas e de viabilidade celular.

## Descrição do projeto

Iniciei o projeto com as [Análises exploratórias](https://github.com/luancsoliver/imersao-dados-desafio-final/blob/main/Notebooks/Analise_exploratoria.ipynb) a partir daí eu iniciei o planejamento do projeto, fiz uma pesquisa sobre a importância das substâncias que mais tiveram ativação provocada pelos compostos e, pela listagem, as que mais foram ativadas foram os inibidores de NF-KB e Proteassoma. Com isso eu quis saber como a ativação destes inibidores afetavam as células. Primeiramente testei com o tipo celular c-0 e depois tirei uma média da resposta de todos os tipos celulares e analisei a resposta que seguiu o mesmo padrão. Encontrei uma resposta significativa das células quando estes inibidores eram ativados. Portanto, a importância deles já se mostrou clara para mim para estes dados. Então achei que seria interessante prever sua ativação utilizando Machine Learning.
