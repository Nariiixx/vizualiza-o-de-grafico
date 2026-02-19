<h2>Sobre o projeto</h2>
<h3>o projeto é um vizualização de gráfico onde eu coloquei em prática o que eu aprendi no cursinho sobre dados</h3>
<h3>tecnolgias usadas:</h3>
<ul>python 3.x</ul>
<ul>pandas</ul>
<ul>seaborn</ul>
<ul>matplotlib</ul>
<p></p>
<h3>código final:</h3>
<p>plt.figure()</p>
<p>plt.subplot(1, 2, 1)</p>
<p>srn.histplot(data.PIB, kde=True, bins=10).set(title='PIB')</p>
<br>
<p>plt.subplot(1, 2, 2)</p>
<p>srn.histplot(data.VALOREMPENHO, kde=True, bins=10).set(title='valor empenho')</p>
<br>
<p>agrupado = data.sort_values('PIB').head(10)</p>
<p>agrupado = agrupado.iloc[:,1:3]</p>
<p>agrupado.plot.bar(x='MUNICIPIO', y='PIB', color='gray').set(title='10 municípios com  PIB')</p>
<br>
<p>agrupado = data.sort_values('VALOREMPENHO').head(10)</p>
<p>agrupado = agrupado.iloc[:,[1,3]]</p>
<p>agrupado.plot.bar(x='MUNICIPIO', y='VALOREMPENHO', color='gray').set(title='10 municípios com valor empenho')</p>

