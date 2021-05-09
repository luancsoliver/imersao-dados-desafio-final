![imagem do título](https://www.wreducacional.com.br/img_cursos/prod/img_1230x644/saude/farmacologia.jpg)

# Desenvolvendo um modelo para prever ativação dos inibidores NF-KB e Proteassoma

## Introdução

NF-KB é um complexo proteico que desempenha funções relacionadas com fator de transcrição. Ele é encontrado em quase todos os tipos de células animais e está envolvido com a resposta celular à estímulos de estresse. [mais informações clique aqui](https://pt.wikipedia.org/wiki/NF-%CE%BAB). NF-KB regulam vários processos fisiológicos importantes, incluindo inflamação e respostas imunológicas, crescimento celular, apoteose e a expressão de certos genes virais. Portanto, a via de sinalização NF-KB também forneceu um foco para intervenção farmacológica, principalmente em situações de inflamação crônica ou em câncer, onde a via é frequentemente constitutivamente ativa e desempenha um papel fundamental na doença. [acesse o artigo para mais informações](https://www.nature.com/articles/1209982.pdf).

Proteassoma é um complexo proteico responsável pela degradação de proteínas itracelulares desempenhando um papel central na homeostase proteica por regular diversos processos celulares. [mais informações clique aqui](http://redoxoma.iq.usp.br/paginas_view.php?idPagina=935#.YJfsJSZv81I). Ela é usada para destruir proteínas danificadas ou com erros de síntese, as quais são marcadas para degradação através da ligação de cadeias de [ubiquitina](https://pt.wikipedia.org/wiki/Ubiquitina) em série. É importante que a célula destrua essas proteínas pois elas são potencialmente perigosas. [mais informações clique aqui](https://pt.wikipedia.org/wiki/Proteassoma).

Os inibidores de proteassoma são uma classe importante de medicamentos para o tratamento de [mieloma múltiplo](https://www.abrale.org.br/doencas/mieloma-multiplo/o-que-e/) e [linfoma de células do manto](https://www.abrale.org.br/doencas/linfomas/lnh/subtipos/linfoma-do-manto/o-que-e/) e estão sendo investigados para outras doenças. Enquanto inibidores de NF-KB estão sendo estudados para tratamento de certos tipos de câncer e doenças neodegenerativas e inflamatórias. [acesse o artigo para mais informações](https://www.nature.com/articles/1209982.pdf).

## Fonte de Dados

Os dados usados neste projetos originaram do Laboratory innovation science at Harvard. Os dados foram levantados de 23.813 amostras onde foram testados 3.289 tipos de compostos que podem dar origem à fármacos. Obtiveram dados de expressão gênica de 772 genes e de viabilidade celular de 100 tipos celulares. A partir desses dados ele podem prever a reação do organismo aos compostos e criar diferentes tipos de drogas para uso de humanos.

Com os dados iniciais sobre o efeito dos compostos sobre os genes e células testou-se a ativação de 206 diferentes substâncias. É aqui que entra os inbidores de NF-KB e Proteassoma.

Toda a descrição e representação do data frame estão em [Análises exploratórias](https://github.com/luancsoliver/imersao-dados-desafio-final/blob/main/Notebooks/Analise_exploratoria.ipynb).

## Objetivos

Esse projeto visa mostrar a importância destes dois inibidores na farmacologia, mostrar como a ativação deles afeta culturas celulares e criar um modelo de Machine Learning que consegue prever a ativação destes inibidores com as informações genéticas e de viabilidade celular.

## Descrição do projeto

O projeto se baseou na importânca dos inibidores para o experimento como um todo. Nas [Análises exploratórias](https://github.com/luancsoliver/imersao-dados-desafio-final/blob/main/Notebooks/Analise_exploratoria.ipynb) eu defini os inibidores a serem estudados e a partir daí quis saber qual a relação entre a ativação deles e a viabilidade celular. Com o desenvolver dessa ideia achei que seria interessante termos um modelo de ML (Machine Learning) que conseguisse prever a ativação destes inibidores tão importantes. Com isso gerei os modelos que são descritos nas [Análises exploratórias](https://github.com/luancsoliver/imersao-dados-desafio-final/blob/main/Notebooks/Analise_exploratoria.ipynb).
Definido tudo que seria feito fiz a [Análise final](https://github.com/luancsoliver/imersao-dados-desafio-final/blob/main/Notebooks/Analise_final.ipynb) reunindo tudo que obti com as análises exploratórias e concluí o projeto com um modelo com alta porcentagem de previsão.

## Conclusão

Os inibidores de NF-KB e Proteassoma foram de essencial importância nesse experimento. O composto mais utiliazado (87d714366) tinha a ativação destes dois inibidores. Tiveram efeito significativo na diminuição da viabilidade celular de todos os tipos de células.

Os modelos que gerei tiveram alto índice de predição, sendo que o modelo do Inibidor de NF-KB teve porcentagem de acerto de 99,16% e o modelo do Inibidor de Proteassoma de 99,47%. As principais variáveis para predição dos modelos foram os valores genéticos, principalmente para o modelo do Inibidor de Proteassoma.
