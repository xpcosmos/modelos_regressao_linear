# Introdução

Esse projeto teve o objetivo de criar um projeto de previsão linear para preços de seguros. O método de regressão linear é base para muitos modelos de machine learning mais complexos e o seu entendimento ajuda a construir uma gama de conhecimentos que ajudarão futuramente em outros experimentos.

# Insights

* O número de crianças aumenta o valor do seguro
* O valor do seguro de pessoas fumantes é consideravelmente mais alto do que aqueles que não fumam
* A idade mostra uma relação linear com o valor do seguro

# Resultados

O modelo obteve uma performance relavante alcançando o R² 82.19% e um R-quadrático de 1317 após um processo de seleção de atributos. A média dos resíduos (erros) foi de 27.62 com um desvio padrão de 1319, valor este justificado por alguns outliers, no entanto, o quantils de 25% e 75% ficaram entre -584 e 258, respectivamente. A distribuição dos resíduos seguiram uma normal, o que aponta que os resíduos não apresetaram underfitting nem overfitting.

## Escolha de atributos

A imagem abaixo demonstra a matriz de correlação gerada após a retirada de outliers considerando um quantil de 75%. O atributo BMI apresentou uma alta correlação com a variável dependente, todavia após a limpeza essa correlação não se manteve. Em primeiros teste a variável já havia sido desconsiderada por apresentar multicolinearidade com outras variável, o que implicaria em uma má generalização do modelo e overfitting. 

![corr](https://github.com/xpcosmos/modelos_regressao_linear/blob/main/preco-seguros/assets/corr.png)

## Erros obitidos 

Para constatar a boa performance do modelo é necessário que os resíduos gerados além da pespectiva numérica. Nas figuras abaixo os dados demonstram aleatoriedade na distribuição dos erros para o junto de teste, outro indicador de boa perfomance do modelo, além dos dados seguirem aproximadamente uma curva normal, afirmação reforçada pelo gráfico QQ-Plot

![dict](https://github.com/xpcosmos/modelos_regressao_linear/blob/main/preco-seguros/assets/distribuicao.png) ![scatter](https://github.com/xpcosmos/modelos_regressao_linear/blob/main/preco-seguros/assets/scatterplot.png)

# Conclusão

O modelo teve análise e resultados satisfatórios ao ponto de vista estatístico, pois obteve uma boa performance nas principais análises, tanto estatísticas quanto visuais.

# Tecnologias utilizadas

* Python
* Sklearn
* Bash/Linux/Unix
* Estatística
* Regressão Linear
* Statsmodels
* Seaborn
* Matplotlib
* Numpy
* Pandas
* Git/Github
* CSV


# Autor

<p align="left">
  <a href="malito:mikeias.d.s.o@gmail.com" alt="Gmail">
  <img src="https://img.shields.io/badge/-Gmail-FF0000?style=flat-square&labelColor=FF0000&logo=gmail&logoColor=white&link=LINK-DO-SEU-EMAIL" /></a>

  <a href="https://www.linkedin.com/in/mikeias-d-s-o/" alt="Linkedin">
  <img src="https://img.shields.io/badge/-Linkedin-0e76a8?style=flat-square&logo=Linkedin&logoColor=white&link=LINK-DO-SEU-LINKEDIN" /></a>

</p>  


# Licença
  
MIT License

Copyright (c) 2022 Mikeias Oliveira

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
